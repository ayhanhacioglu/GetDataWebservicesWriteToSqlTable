# GetDataWebservicesWriteToSqlTable
How to get data from authorized Webservices and write to SQL table with scheduled tasks.
/***********************************************************************************************************************************************/
/*                                                                                                                                             */
/* Please be sure first of all to activate this feature on your SQL Server                                                                     */
/* ----------------------------                                                                                                                */
/* sp_configure 'show advanced options', 1                                                                                                     */
/* GO                                                                                                                                          */
/* RECONFIGURE                                                                                                                                 */
/* GO                                                                                                                                          */
/* sp_configure 'Ole Automation Procedures', 1                                                                                                 */
/* GO                                                                                                                                          */
/* RECONFIGURE                                                                                                                                 */
/* GO                                                                                                                                          */
/* ----------------------------                                                                                                                */
/* This procedure is calling from XCorp B2B Report Webservices api                                                                             */
/* You must be sure all informations of data source from webservices details and you must be sure the accessability to webservices links       */
/* You must create a table on your database with such as end of the this procedure with JSON data type. It must name is XCorpB2BSalesReport.   */
/*                                                                                                                                             */
/* History:                                                                                                                                    */
/* Version Date Person Description                                                                                                             */
/* 1.0     08/08/2023  AH Started                                                                                                              */
/*                                                                                                                                             */
/* Comments:                                                                                                                                   */
/*                                                                                                                                             */
/* https://learn.microsoft.com/en-us/sql/relational-databases/json/json-data-sql-server?view=sql-server-ver16                                  */
/* https://learn.microsoft.com/en-us/sql/relational-databases/json/format-query-results-as-json-with-for-json-sql-server?view=sql-server-ver16 */
/*                                                                                                                                             */
/*                                                                                                                                             */
/* Aliases:                                                                                                                                    */
/* AH : Ayhan HACIOGLU ayhanhacioglu@gmail.com                                                                                                 */
/***********************************************************************************************************************************************/
