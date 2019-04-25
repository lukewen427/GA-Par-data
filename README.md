Data Description
===================================
* risksecuritygoal.json
* risktechnology.json
* services.txt
    * For each row
	* The 1st column: service id
	* The 2nd column: set time
	* The 3rd or more column: technology list
* time.txt
    * It only has 1 column, its x's row corresponds to the local time of x's service in the file services.txt
* combinedata.txt
    * This file combine above serveral files, and it also includes the calculation of risk value and technology value. Details are as follows.
    * For each row, it has several information types, and these types are seperated by \t. And some of these information types contain more information, each of them are seperated by \s,
	* The 1st type: service id
	* The 2nd type: local time
	* The 3rd type: set time
	* The 4th type: technology list
	* The 5th type: risk value information. It is seperated by \s, and its value based on the order "R1, R2, R3, R4, R5, R6, R7, R8, R9"
	* The 6th type: goal value information. It is also seperated by \s, and its value based on the order "Accountability, Audibility, Authenticity, Availability, Confidentiality, Integrity, Non-repudiation, Privacy"
	* The 7th type: The total value of this service
* sub-combinedata-*.csv
    * sub-combinedata-1.csv:
        * service id, local time, set time, technology list
    * sub-combinedata-2.csv:
        * service id, risk value information. Its value based on the order "R1, R2, R3, R4, R5, R6, R7, R8, R9"
    * sub-combinedata-3.csv:
        * service id, goal value information. Its value based on the order "Accountability, Audibility, Authenticity, Availability, Confidentiality, Integrity, Non-repudiation, Privacy"
