# Data-Wharehouse-Model
Conceptual Model of a Data Warehouse Application in a Bus Paycheck Contex

# Delimiters
The database should include drivers, identified by their CPFs, RGs, addresses, date of birth, driver's license numbers, and bank account information for payment, as well as passengers, identified by their CPFs, RGs, addresses, date of birth, and credit card numbers. In addition to them, attendants should be registered, identified by their CPFs, RGs, addresses, date of birth, and educational background. Drivers and attendants can use transportation services as passengers. An attendant can also be a driver during idle hours. One or more vehicles are associated with a driver, where each vehicle should be identified by its RENAVAM number, purchase date, brand, model, year, price, and characteristic, which should be one of {economic, SUV, luxury, rural}.

An insurance company is identified by a CNPJ, name, telephone, and postal address. An insurance company may be responsible for one or more vehicle insurances, identified by policy number and value. The system does not store the vehicle insurance policy history; therefore, at most, only a single policy number per vehicle appears in the system at a time. A ride is recorded as a service provided by a driver to multiple passengers, identified by the ride number, destination address, start date, end date, start time, end time, total ride value, and ride price per passenger. An attendant is linked to the support of each ride, where passengers can send inquiries, identified by a sequential number, question text, and response text, to the attendant during the ride. The system stores the ride history. Company transportation managers need to perform analytical queries on the database to know travel statistics by driver, location, passenger, and date. That is, the database should be able to answer questions such as "What is the number of trips by Driver 'Daniel de Oliveira' in January/2020?" or "What is the average number of trips in the year whose destination is Passo da Pátria Street in Niterói?"

## OLTP
![ER_Conceitual_OLTP (1)](https://github.com/hugoles/Data-Wharehouse-Model/assets/67278688/3cc3fb44-f5c7-4c7f-b5b4-cd8736da019d)






## OLAP
![ER_Conceitual_OLAP (1)](https://github.com/hugoles/Data-Wharehouse-Model/assets/67278688/267d3369-f925-4d7b-aeb3-80b7bf464b3b)
