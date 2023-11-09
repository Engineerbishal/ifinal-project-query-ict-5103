CREATE DATABASE ICT5103finalproject;
USE ICT5103finalproject;

CREATE TABLE  Worker (
    WorkerID VARCHAR(100) PRIMARY KEY,
    Name VARCHAR(100),
    Department VARCHAR(100),
    Gender VARCHAR(10),
    Salary DECIMAL(10, 2),
    JoiningDate DATE,
    WorkSlot VARCHAR(100),
    DailyOutput INT,
    Plant VARCHAR(100),
    SupervisorID VARCHAR(100)
);


CREATE TABLE  Supervisor (
    SupervisorID VARCHAR(100) PRIMARY KEY,
    Name VARCHAR(100),
    Gender VARCHAR(10),
    Plant VARCHAR(100),
    WorkSlot VARCHAR(100),
    Department VARCHAR(100),
    JoiningDate DATE,
    Salary DECIMAL(10, 2)
);


CREATE TABLE  Product (
    ProductID VARCHAR(100) PRIMARY KEY,
    WorkerID VARCHAR(100),
    SupervisorID VARCHAR(100)
);


INSERT INTO Worker ( WorkerID, Name, Department, Gender, Salary, JoiningDate, WorkSlot, DailyOutput, Plant, SupervisorID)
VALUES 
    ('W1', 'Rahim', 'T-shirt', 'Male', 35000, '2017-01-01', 'Morning', 5, 'Plant1', 'S1'),
    ('W2', 'Karim', 'T-shirt', 'Female', 38000, '2017-01-01', 'Morning', 5, 'Plant1', 'S1'),
    ('W3', 'Hasan', 'T-shirt', 'Male', 40000, '2017-01-01', 'Morning', 5, 'Plant1', 'S1'),
    ('W4', 'Ayesha', 'T-shirt', 'Female', 33000, '2017-01-01', 'Morning', 5, 'Plant1', 'S1'),
    ('W5', 'Fatima', 'T-shirt', 'Male', 37000, '2017-01-01', 'Morning', 5, 'Plant1', 'S1'),
    ('W6', 'Abdullah', 'T-shirt', 'Male', 36000, '2017-01-01', 'Morning', 5, 'Plant1', 'S2'),
    ('W7', 'Fahima', 'T-shirt', 'Female', 39000, '2017-01-01', 'Morning', 5, 'Plant1', 'S2'),
    ('W8', 'Mamun', 'T-shirt', 'Male', 40000, '2017-01-01', 'Morning', 5, 'Plant1', 'S2'),
    ('W9', 'Sabina', 'T-shirt', 'Female', 34000, '2017-01-01', 'Morning', 5, 'Plant1', 'S2'),
    ('W10', 'Kamal', 'T-shirt', 'Male', 38000, '2017-01-01', 'Morning', 5, 'Plant1', 'S2');


INSERT INTO Supervisor (SupervisorID,Name, Gender, Plant, WorkSlot, Department, JoiningDate, Salary)
VALUES 
    ('S1', 'Mahmud', 'Male', 'Plant1', 'Morning', 'T-shirt', '2017-01-01', 75000),
    ('S2', 'Rashid', 'Male', 'Plant1', 'Morning', 'T-shirt', '2017-01-01', 75000);

INSERT INTO Product (ProductID, WorkerID, SupervisorID)
VALUES 
    ('P1', 'W1', 'S1'),
    ('P2', 'W1', 'S1'),
    ('P3', 'W1', 'S1'),
    ('P4', 'W1', 'S1'),
    ('P5', 'W1', 'S1'),
    ('P6', 'W2', 'S1'),
    ('P7', 'W2', 'S1'),
    ('P8', 'W2', 'S1'),
    ('P9', 'W2', 'S1'),
    ('P10', 'W2', 'S1'),
    ('P11', 'W3', 'S1'),
    ('P12', 'W3', 'S1'),
    ('P13', 'W3', 'S1'),
    ('P14', 'W3', 'S1'),
    ('P15', 'W3', 'S1'),
    ('P16', 'W4', 'S1'),
    ('P17', 'W4', 'S1'),
    ('P18', 'W4', 'S1'),
    ('P19', 'W4', 'S1'),
    ('P20', 'W4', 'S1'),
    ('P21', 'W5', 'S1'),
    ('P22', 'W5', 'S1'),
    ('P23', 'W5', 'S1'),
    ('P24', 'W5', 'S1'),
    ('P25', 'W5', 'S1'),
    ('P26', 'W6', 'S2'),
    ('P27', 'W6', 'S2'),
    ('P28', 'W6', 'S2'),
    ('P29', 'W6', 'S2'),
    ('P30', 'W6', 'S2'),
    ('P31', 'W7', 'S2'),
    ('P32', 'W7', 'S2'),
    ('P33', 'W7', 'S2'),
    ('P34', 'W7', 'S2'),
    ('P35', 'W7', 'S2'),
    ('P36', 'W8', 'S2'),
    ('P37', 'W8', 'S2'),
    ('P38', 'W8', 'S2'),
    ('P39', 'W8', 'S2'),
    ('P40', 'W8', 'S2'),
    ('P41', 'W9', 'S2'),
    ('P42', 'W9', 'S2'),
    ('P43', 'W9', 'S2'),
    ('P44', 'W9', 'S2'),
    ('P45', 'W9', 'S2'),
    ('P46', 'W10', 'S2'),
    ('P47', 'W10', 'S2'),
    ('P48', 'W10', 'S2'),
    ('P49', 'W10', 'S2'),
    ('P50', 'W10', 'S2');




INSERT INTO Worker (WorkerID, Name, Department, Gender, Salary, JoiningDate, WorkSlot, DailyOutput, Plant, SupervisorID)
VALUES 
    ('W11', 'Jamal', 'T-shirt', 'Male', 36000, '2017-01-01', 'Morning', 5, 'Plant1', 'S3'),
    ('W12', 'Roksana', 'T-shirt', 'Female', 39000, '2017-01-01', 'Morning', 5, 'Plant1', 'S3'),
    ('W13', 'Anwar', 'T-shirt', 'Male', 40000, '2017-01-01', 'Morning', 5, 'Plant1', 'S3'),
    ('W14', 'Shabnam', 'T-shirt', 'Female', 34000, '2017-01-01', 'Morning', 5, 'Plant1', 'S3'),
    ('W15', 'Iqbal', 'T-shirt', 'Male', 38000, '2017-01-01', 'Morning', 5, 'Plant1', 'S3'),
    ('W16', 'Sohel', 'T-shirt', 'Male', 36000, '2017-01-01', 'Morning', 5, 'Plant1', 'S4'),
    ('W17', 'Rahima', 'T-shirt', 'Female', 39000, '2017-01-01', 'Morning', 5, 'Plant1', 'S4'),
    ('W18', 'Rafiq', 'T-shirt', 'Male', 40000, '2017-01-01', 'Morning', 5, 'Plant1', 'S4'),
    ('W19', 'Salma', 'T-shirt', 'Female', 34000, '2017-01-01', 'Morning', 5, 'Plant1', 'S4'),
    ('W20', 'Babul', 'T-shirt', 'Male', 38000, '2017-01-01', 'Morning', 5, 'Plant1', 'S4');




INSERT INTO Supervisor (SupervisorID, Name, Gender, Plant, WorkSlot, Department, JoiningDate, Salary)
VALUES 
    ('S3', 'Salim', 'Male', 'Plant1', 'Morning', 'T-shirt', '2017-01-01', 75000),
    ('S4', 'Karim', 'Male', 'Plant1', 'Morning', 'T-shirt', '2017-01-01', 75000);









INSERT INTO Product (ProductID, WorkerID, SupervisorID)
VALUES 
    ('P51', 'W11', 'S3'),
    ('P52', 'W11', 'S3'),
    ('P53', 'W11', 'S3'),
    ('P54', 'W11', 'S3'),
    ('P55', 'W11', 'S3'),
    ('P56', 'W12', 'S3'),
    ('P57', 'W12', 'S3'),
    ('P58', 'W12', 'S3'),
    ('P59', 'W12', 'S3'),
    ('P60', 'W12', 'S3'),
    ('P61', 'W13', 'S3'),
    ('P62', 'W13', 'S3'),
    ('P63', 'W13', 'S3'),
    ('P64', 'W13', 'S3'),
    ('P65', 'W13', 'S3'),
    ('P66', 'W14', 'S3'),
    ('P67', 'W14', 'S3'),
    ('P68', 'W14', 'S3'),
    ('P69', 'W14', 'S3'),
    ('P70', 'W14', 'S3'),
    ('P71', 'W15', 'S3'),
    ('P72', 'W15', 'S3'),
    ('P73', 'W15', 'S3'),
    ('P74', 'W15', 'S3'),
    ('P75', 'W15', 'S3'),
    ('P76', 'W16', 'S4'),
    ('P77', 'W16', 'S4'),
    ('P78', 'W16', 'S4'),
    ('P79', 'W16', 'S4'),
    ('P80', 'W16', 'S4'),
    ('P81', 'W17', 'S4'),
    ('P82', 'W17', 'S4'),
    ('P83', 'W17', 'S4'),
    ('P84', 'W17', 'S4'),
    ('P85', 'W17', 'S4'),
    ('P86', 'W18', 'S4'),
    ('P87', 'W18', 'S4'),
    ('P88', 'W18', 'S4'),
    ('P89', 'W18', 'S4'),
    ('P90', 'W18', 'S4'),
    ('P91', 'W19', 'S4'),
    ('P92', 'W19', 'S4'),
    ('P93', 'W19', 'S4'),
    ('P94', 'W19', 'S4'),
    ('P95', 'W19', 'S4'),
    ('P96', 'W20', 'S4'),
    ('P97', 'W20', 'S4'),
    ('P98', 'W20', 'S4'),
    ('P99', 'W20', 'S4'),
    ('P100', 'W20', 'S4');
    
    
    
    
    
    
INSERT INTO Worker (WorkerID, Name, Department, Gender, Salary, JoiningDate, WorkSlot, DailyOutput, Plant, SupervisorID)
VALUES 
    ('W21', 'Asif', 'T-shirt', 'Male', 36000, '2017-01-01', 'Morning', 5, 'Plant2', 'S5'),
    ('W22', 'Nasima', 'T-shirt', 'Female', 39000, '2017-01-01', 'Morning', 5, 'Plant2', 'S5'),
    ('W23', 'Shahid', 'T-shirt', 'Male', 40000, '2017-01-01', 'Morning', 5, 'Plant2', 'S5'),
    ('W24', 'Rabeya', 'T-shirt', 'Female', 34000, '2017-01-01', 'Morning', 5, 'Plant2', 'S5'),
    ('W25', 'Rafiqul', 'T-shirt', 'Male', 38000, '2017-01-01', 'Morning', 5, 'Plant2', 'S5'),
    ('W26', 'Shafiq', 'T-shirt', 'Male', 36000, '2017-01-01', 'Morning', 5, 'Plant2', 'S6'),
    ('W27', 'Tahmina', 'T-shirt', 'Female', 39000, '2017-01-01', 'Morning', 5, 'Plant2', 'S6'),
    ('W28', 'Ruhul', 'T-shirt', 'Male', 40000, '2017-01-01', 'Morning', 5, 'Plant2', 'S6'),
    ('W29', 'Farida', 'T-shirt', 'Female', 34000, '2017-01-01', 'Morning', 5, 'Plant2', 'S6'),
    ('W30', 'Mizan', 'T-shirt', 'Male', 38000, '2017-01-01', 'Morning', 5, 'Plant2', 'S6');
    
    
    

INSERT INTO Supervisor (SupervisorID, Name, Gender, Plant, WorkSlot, Department, JoiningDate, Salary)
VALUES 
    ('S5', 'Rafiqul', 'Male', 'Plant2', 'Morning', 'T-shirt', '2017-01-01', 75000),
    ('S6', 'Rashed', 'Male', 'Plant1', 'Night', 'T-shirt', '2017-01-01', 75000);


INSERT INTO Product (ProductID, WorkerID, SupervisorID)
VALUES 
    ('P101', 'W21', 'S5'),
    ('P102', 'W21', 'S5'),
    ('P103', 'W21', 'S5'),
    ('P104', 'W21', 'S5'),
    ('P105', 'W21', 'S5'),
    ('P106', 'W22', 'S5'),
    ('P107', 'W22', 'S5'),
    ('P108', 'W22', 'S5'),
    ('P109', 'W22', 'S5'),
    ('P110', 'W22', 'S5'),
    ('P111', 'W23', 'S5'),
    ('P112', 'W23', 'S5'),
    ('P113', 'W23', 'S5'),
    ('P114', 'W23', 'S5'),
    ('P115', 'W23', 'S5'),
    ('P116', 'W24', 'S5'),
    ('P117', 'W24', 'S5'),
    ('P118', 'W24', 'S5'),
    ('P119', 'W24', 'S5'),
    ('P120', 'W24', 'S5'),
    ('P121', 'W25', 'S5'),
    ('P122', 'W25', 'S5'),
    ('P123', 'W25', 'S5'),
    ('P124', 'W25', 'S5'),
    ('P125', 'W25', 'S5'),
    ('P126', 'W26', 'S6'),
    ('P127', 'W26', 'S6'),
    ('P128', 'W26', 'S6'),
    ('P129', 'W26', 'S6'),
    ('P130', 'W26', 'S6'),
    ('P131', 'W27', 'S6'),
    ('P132', 'W27', 'S6'),
    ('P133', 'W27', 'S6'),
    ('P134', 'W27', 'S6'),
    ('P135', 'W27', 'S6'),
    ('P136', 'W28', 'S6'),
    ('P137', 'W28', 'S6'),
    ('P138', 'W28', 'S6'),
    ('P139', 'W28', 'S6'),
    ('P140', 'W28', 'S6'),
    ('P141', 'W29', 'S6'),
    ('P142', 'W29', 'S6'),
    ('P143', 'W29', 'S6'),
    ('P144', 'W29', 'S6'),
    ('P145', 'W29', 'S6'),
    ('P146', 'W30', 'S6'),
    ('P147', 'W30', 'S6'),
    ('P148', 'W30', 'S6'),
    ('P149', 'W30', 'S6'),
    ('P150', 'W30', 'S6');
    
    
    
    
    
    
  
INSERT INTO Worker (WorkerID, Name, Department, Gender, Salary, JoiningDate, WorkSlot, DailyOutput, Plant, SupervisorID)
VALUES 
   
    ('W31', 'Sajid', 'T-shirt', 'Male', 36000, '2017-01-01', 'Night', 5, 'Plant1', 'S7'),
    ('W32', 'Farzana', 'T-shirt', 'Female', 39000, '2017-01-01', 'Night', 5, 'Plant1', 'S7'),
    ('W33', 'Rakib', 'T-shirt', 'Male', 40000, '2017-01-01', 'Night', 5, 'Plant1', 'S7'),
    ('W34', 'Jahanara', 'T-shirt', 'Female', 34000, '2017-01-01', 'Night', 5, 'Plant1', 'S7'),
    ('W35', 'Shamim', 'T-shirt', 'Male', 38000, '2017-01-01', 'Night', 5, 'Plant1', 'S7'),
    ('W36', 'Sakib', 'T-shirt', 'Male', 36000, '2017-01-01', 'Night', 5, 'Plant1', 'S8'),
    ('W37', 'Shamima', 'T-shirt', 'Female', 39000, '2017-01-01', 'Night', 5, 'Plant1', 'S8'),
    ('W38', 'Rasel', 'T-shirt', 'Male', 40000, '2017-01-01', 'Night', 5, 'Plant1', 'S8'),
    ('W39', 'Jesmin', 'T-shirt', 'Female', 34000, '2017-01-01', 'Night', 5, 'Plant1', 'S8'),
    ('W40', 'Ripon', 'T-shirt', 'Male', 38000, '2017-01-01', 'Night', 5, 'Plant1', 'S8');


INSERT INTO Supervisor (SupervisorID, Name, Gender, Plant, WorkSlot, Department, JoiningDate, Salary)
VALUES 
    
    ('S7', 'Rashed', 'Male', 'Plant1', 'Night', 'T-shirt', '2017-01-01', 75000);
    
    INSERT INTO Supervisor (SupervisorID, Name, Gender, Plant, WorkSlot, Department, JoiningDate, Salary)
VALUES 
    ('S8', 'Shahidul',  'Male', 'Plant1', 'Night', 'T-shirt', '2017-01-01', 75000 );


INSERT INTO Product (ProductID, WorkerID, SupervisorID)
VALUES 
    
    ('P151', 'W31', 'S7'),
    ('P152', 'W31', 'S7'),
    ('P153', 'W31', 'S7'),
    ('P154', 'W31', 'S7'),
    ('P155', 'W31', 'S7'),
    ('P156', 'W32', 'S7'),
    ('P157', 'W32', 'S7'),
    ('P158', 'W32', 'S7'),
    ('P159', 'W32', 'S7'),
    ('P160', 'W32', 'S7'),
    ('P161', 'W33', 'S7'),
    ('P162', 'W33', 'S7'),
    ('P163', 'W33', 'S7'),
    ('P164', 'W33', 'S7'),
    ('P165', 'W33', 'S7'),
    ('P166', 'W34', 'S7'),
    ('P167', 'W34', 'S7'),
    ('P168', 'W34', 'S7'),
    ('P169', 'W34', 'S7'),
    ('P170', 'W34', 'S7'),
    ('P171', 'W35', 'S7'),
    ('P172', 'W35', 'S7' ),
    ('P173', 'W35', 'S7'),
    ('P174', 'W35', 'S7'),
    ('P175', 'W35', 'S7'),
    ('P176', 'W36', 'S8'),
    ('P177', 'W36', 'S8'),
    ('P178', 'W36', 'S8'),
    ('P179', 'W36', 'S8'),
    ('P180', 'W36', 'S8'),
    ('P181', 'W37', 'S8'),
    ('P182', 'W37', 'S8'),
    ('P183', 'W37', 'S8'),
    ('P184', 'W37', 'S8'),
    ('P185', 'W37', 'S8'),
    ('P186', 'W38', 'S8'),
    ('P187', 'W38', 'S8'),
    ('P188', 'W38', 'S8'),
    ('P189', 'W38', 'S8'),
    ('P190', 'W38', 'S8'),
    ('P191', 'W39', 'S8'),
    ('P192', 'W39', 'S8'),
    ('P193', 'W39', 'S8'),
    ('P194', 'W39', 'S8'),
    ('P195', 'W39', 'S8'),
    ('P196', 'W40', 'S8'),
    ('P197', 'W40', 'S8'),
    ('P198', 'W40', 'S8'),
    ('P199', 'W40', 'S8'),
    ('P200', 'W40', 'S8');
    
















INSERT INTO Worker (WorkerID, Name, Department, Gender, Salary, JoiningDate, WorkSlot, DailyOutput, Plant, SupervisorID)
VALUES 
   
    ('W41', 'Rafiq', 'T-shirt', 'Male', 36000, '2017-01-01', 'Night', 5, 'Plant2', 'S9'),
    ('W42', 'Shahana', 'T-shirt', 'Female', 39000, '2017-01-01', 'Night', 5, 'Plant2', 'S9'),
    ('W43', 'Kamrul', 'T-shirt', 'Male', 40000, '2017-01-01', 'Night', 5, 'Plant2', 'S9'),
    ('W44', 'Roksana', 'T-shirt', 'Female', 34000, '2017-01-01', 'Night', 5, 'Plant2', 'S9'),
    ('W45', 'Shahjahan', 'T-shirt', 'Male', 38000, '2017-01-01', 'Night', 5, 'Plant2', 'S9'),
    ('W46', 'Shakil', 'T-shirt', 'Male', 36000, '2017-01-01', 'Night', 5, 'Plant2', 'S10'),
    ('W47', 'Shahina', 'T-shirt', 'Female', 39000, '2017-01-01', 'Night', 5, 'Plant2', 'S10'),
    ('W48', 'Rony', 'T-shirt', 'Male', 40000, '2017-01-01', 'Night', 5, 'Plant2', 'S10'),
    ('W49', 'Shahnaz', 'T-shirt', 'Female', 34000, '2017-01-01', 'Night', 5, 'Plant2', 'S10'),
    ('W50', 'Shamim', 'T-shirt', 'Male', 38000, '2017-01-01', 'Night', 5, 'Plant2', 'S10');


INSERT INTO Supervisor (SupervisorID, Name, Gender, Plant, WorkSlot, Department, JoiningDate, Salary)
VALUES 
    
    ('S9', 'Mominul', 'Male', 'Plant2', 'Night', 'T-shirt', '2017-01-01', 75000),
    ('S10', 'Mehedi', 'Male', 'Plant2', 'Night', 'T-shirt', '2017-01-01', 75000);
    
    
    
    INSERT INTO Product (ProductID, WorkerID, SupervisorID)
VALUES 
    
    ('P201', 'W41', 'S9'),
    ('P202', 'W41', 'S9'),
    ('P203', 'W41', 'S9'),
    ('P204', 'W41', 'S9'),
    ('P205', 'W41', 'S9'),
    ('P206', 'W42', 'S9'),
    ('P207', 'W42', 'S9'),
    ('P208', 'W42', 'S9'),
    ('P209', 'W42', 'S9'),
    ('P210', 'W42', 'S9'),
    ('P211', 'W43', 'S9'),
    ('P212', 'W43', 'S9'),
    ('P213', 'W43', 'S9'),
    ('P214', 'W43', 'S9'),
    ('P215', 'W43', 'S9'),
    ('P216', 'W44', 'S9'),
    ('P217', 'W44', 'S9'),
    ('P218', 'W44', 'S9'),
    ('P219', 'W44', 'S9'),
    ('P220', 'W44', 'S9'),
    ('P221', 'W45', 'S9'),
    ('P222', 'W45', 'S9' ),
    ('P223', 'W45', 'S9'),
    ('P224', 'W45', 'S9'),
    ('P225', 'W45', 'S10'),
    ('P226', 'W46', 'S10'),
    ('P227', 'W46', 'S10'),
    ('P228', 'W46', 'S10'),
    ('P229', 'W46', 'S10'),
    ('P230', 'W46', 'S10'),
    ('P231', 'W47', 'S10'),
    ('P232', 'W47', 'S10'),
    ('P233', 'W47', 'S10'),
    ('P234', 'W47', 'S10'),
    ('P235', 'W47', 'S10'),
    ('P236', 'W48', 'S10'),
    ('P237', 'W48', 'S10'),
    ('P238', 'W48', 'S10'),
    ('P239', 'W48', 'S10'),
    ('P240', 'W48', 'S10'),
    ('P241', 'W49', 'S10'),
    ('P242', 'W49', 'S10'),
    ('P243', 'W49', 'S10'),
    ('P244', 'W49', 'S10'),
    ('P245', 'W49', 'S10'),
    ('P246', 'W50', 'S10'),
    ('P247', 'W50', 'S10'),
    ('P248', 'W50', 'S10'),
    ('P249', 'W50', 'S10'),
    ('P250', 'W50', 'S10');



-- Inserting data into Worker table
INSERT INTO Worker (WorkerID, Name, Department, Gender, Salary, JoiningDate, WorkSlot, DailyOutput, Plant, SupervisorID)
VALUES 
('W51', 'Shahid', 'Jeans', 'Male', 36000, '2017-01-01', 'Morning', 5, 'Plant3', 'S11'),
('W52', 'Rahima', 'Jeans', 'Female', 39000, '2017-01-01', 'Morning', 5, 'Plant3', 'S11'),
('W53', 'Kamrul', 'Jeans', 'Male', 40000, '2017-01-01', 'Morning', 5, 'Plant3', 'S11'),
('W54', 'Jahanara', 'Jeans', 'Female', 34000, '2017-01-01', 'Morning', 5, 'Plant3', 'S11'),
('W55', 'Ripon', 'Jeans', 'Male', 38000, '2017-01-01', 'Morning', 5, 'Plant3', 'S11');

-- Inserting data into Supervisor table
INSERT INTO Supervisor (SupervisorID, Name, Gender, Plant, WorkSlot, Department, JoiningDate, Salary)
VALUES 
('S11-Mehedi', 'Mehedi', 'Male', 'Plant3', 'Morning', 'Jeans', '2017-01-01', 75000);

INSERT INTO Product (ProductID, WorkerID, SupervisorID)
VALUES 
('P251', 'W51', 'S11-Mehedi'),
('P252', 'W51', 'S11-Mehedi'),
('P253', 'W51', 'S11-Mehedi'),
('P254', 'W51', 'S11-Mehedi'),
('P255', 'W51', 'S11-Mehedi'),
('P256', 'W52', 'S11-Mehedi'),
('P257', 'W52', 'S11-Mehedi'),
('P258', 'W52', 'S11-Mehedi'),
('P259', 'W52', 'S11-Mehedi'),
('P260', 'W52', 'S11-Mehedi'),
('P261', 'W53', 'S11-Mehedi'),
('P262', 'W53', 'S11-Mehedi'),
('P263', 'W53', 'S11-Mehedi'),
('P264', 'W53', 'S11-Mehedi'),
('P265', 'W53', 'S11-Mehedi'),
('P266', 'W54', 'S11-Mehedi'),
('P267', 'W54', 'S11-Mehedi'),
('P268', 'W54', 'S11-Mehedi'),
('P269', 'W54', 'S11-Mehedi'),
('P270', 'W54', 'S11-Mehedi'),
('P271', 'W55', 'S11-Mehedi'),
('P272', 'W55', 'S11-Mehedi'),
('P273', 'W55', 'S11-Mehedi'),
('P274', 'W55', 'S11-Mehedi'),
('P275', 'W55', 'S11-Mehedi');










-- Inserting data into Worker table
INSERT INTO Worker (WorkerID, Name, Department, Gender, Salary, JoiningDate, WorkSlot, DailyOutput, Plant, SupervisorID)
VALUES ('W56', 'Shakil', 'Jeans', 'Male', 36000, '2017-01-01', 'Night', 5, 'Plant4', 'S12'),
       ('W57', 'Shahana', 'Jeans', 'Female', 39000, '2017-01-01', 'Night', 5, 'Plant4', 'S12'),
       ('W58', 'Rony', 'Jeans', 'Male', 40000, '2017-01-01', 'Night', 5, 'Plant4', 'S12'),
       ('W59', 'Jahanara', 'Jeans', 'Female', 34000, '2017-01-01', 'Night', 5, 'Plant4', 'S12'),
       ('W60', 'Ripon', 'Jeans', 'Male', 38000, '2017-01-01', 'Night', 5, 'Plant4', 'S12');

-- Inserting data into Supervisor table
INSERT INTO Supervisor (SupervisorID, Name, Gender, Plant, WorkSlot, Department, JoiningDate, Salary)
VALUES ('S12-Rashed', 'Rashed', 'Male', 'Plant4', 'Night', 'Jeans', '2017-01-01', 75000);

-- Inserting data into Product table
INSERT INTO Product (ProductID, WorkerID, SupervisorID)
VALUES ('P276', 'W56', 'S12'),
       ('P277', 'W56', 'S12'),
       ('P278', 'W56', 'S12'),
       ('P279', 'W56', 'S12'),
       ('P280', 'W56', 'S12'),
       ('P281', 'W57', 'S12'),
       ('P282', 'W57', 'S12'),
       ('P283', 'W57', 'S12'),
       ('P284', 'W57', 'S12'),
       ('P285', 'W57', 'S12'),
       ('P286', 'W58', 'S12'),
       ('P287', 'W58', 'S12'),
       ('P288', 'W58', 'S12'),
       ('P289', 'W58', 'S12'),
       ('P290', 'W58', 'S12'),
       ('P291', 'W59', 'S12'),
       ('P292', 'W59', 'S12'),
       ('P293', 'W59', 'S12'),
       ('P294', 'W59', 'S12'),
       ('P295', 'W59', 'S12'),
       ('P296', 'W60', 'S12'),
       ('P297', 'W60', 'S12'),
       ('P298', 'W60', 'S12'),
       ('P299', 'W60', 'S12'),
       ('P300', 'W60', 'S12');

-- Inserting data into Worker table
INSERT INTO Worker (WorkerID, Name, Department, Gender, Salary, JoiningDate, WorkSlot, DailyOutput, Plant, SupervisorID)
VALUES ('W61', 'Shakil', 'Jeans', 'Male', 36000, '2017-01-01', 'Night', 5, 'Plant4', 'S13'),
       ('W62', 'Shahana', 'Jeans', 'Female', 39000, '2017-01-01', 'Night', 5, 'Plant4', 'S13'),
       ('W63', 'Rony', 'Jeans', 'Male', 40000, '2017-01-01', 'Night', 5, 'Plant4', 'S13'),
       ('W64', 'Jahanara', 'Jeans', 'Female', 34000, '2017-01-01', 'Night', 5, 'Plant4', 'S13'),
       ('W65', 'Ripon', 'Jeans', 'Male', 38000, '2017-01-01', 'Night', 5, 'Plant4', 'S13');

-- Inserting data into Supervisor table
INSERT INTO Supervisor (SupervisorID, Name, Gender, Plant, WorkSlot, Department, JoiningDate, Salary)
VALUES ('S13-Mehedi', 'Mehedi', 'Male', 'Plant4', 'Night', 'Jeans', '2017-01-01', 75000);

-- Inserting data into Product table
INSERT INTO Product (ProductID, WorkerID, SupervisorID)
VALUES ('P301', 'W61', 'S13'),
       ('P302', 'W61', 'S13'),
       ('P303', 'W61', 'S13'),
       ('P304', 'W61', 'S13'),
       ('P305', 'W61', 'S13'),
       ('P306', 'W62', 'S13'),
       ('P307', 'W62', 'S13'),
       ('P308', 'W62', 'S13'),
       ('P309', 'W62', 'S13'),
       ('P310', 'W62', 'S13'),
       ('P311', 'W63', 'S13'),
       ('P312', 'W63', 'S13'),
       ('P313', 'W63', 'S13'),
       ('P314', 'W63', 'S13'),
       ('P315', 'W63', 'S13'),
       ('P316', 'W64', 'S13'),
       ('P317', 'W64', 'S13'),
       ('P318', 'W64', 'S13'),
       ('P319', 'W64', 'S13'),
       ('P320', 'W64', 'S13'),
       ('P321', 'W65', 'S13'),
       ('P322', 'W65', 'S13'),
       ('P323', 'W65', 'S13'),
       ('P324', 'W65', 'S13'),
       ('P325', 'W65', 'S13');








SELECT *
FROM Product
JOIN Worker ON Product.WorkerID = Worker.WorkerID
JOIN Supervisor ON Product.SupervisorID = Supervisor.SupervisorID;


SELECT SUM(Worker.Salary) AS TotalSalary
FROM Worker;



SELECT WorkerID, Name, Salary
FROM Worker;




SELECT SupervisorID, Name, Salary
FROM Supervisor;



SELECT SUM(Salary) AS TotalSupervisorsSalary
FROM Supervisor;


SELECT *
FROM Worker
WHERE WorkSlot = 'Night';


SELECT *
FROM Worker
WHERE WorkSlot = 'Morning';



SELECT COUNT(*)
FROM Worker
WHERE Plant = 'Plant1';


SELECT *
FROM Worker
JOIN Product ON Worker.WorkerID = Product.WorkerID;

SELECT COUNT(*) AS TotalJeansProducts
FROM Product P
JOIN Worker W ON P.WorkerID = W.WorkerID
JOIN Supervisor S ON P.SupervisorID = S.SupervisorID
WHERE S.Department = 'Jeans';

SELECT P.ProductID
FROM Product P
JOIN Supervisor S ON P.SupervisorID = S.SupervisorID
WHERE S.Department = 'Jeans';



SELECT P.ProductID
FROM Product P
JOIN Worker W ON P.WorkerID = W.WorkerID
JOIN Supervisor S ON W.SupervisorID = S.SupervisorID
WHERE S.Department = 'Jeans';



SELECT W.*
FROM Worker W
JOIN Supervisor S ON W.SupervisorID = S.SupervisorID
WHERE S.Department = 'Jeans';




SELECT *
FROM Worker
WHERE Department = 'Tshirt';
SELECT WorkerID, Name
FROM Worker
WHERE Department = 'Jeans';




SELECT COUNT(ProductID)
FROM Product
WHERE ProductType = 'Jeans';







SELECT ProductID
FROM Product
WHERE ProductType = 'TShirt';

SELECT W.*
FROM Worker W
JOIN Supervisor S ON W.SupervisorID = S.SupervisorID
WHERE S.Department = 'Tshirt';


SELECT *
FROM Worker
WHERE Department = 'TShirt';
SELECT WorkerID, Name
FROM Worker
WHERE Department = 'Tshirt';






SELECT W.*
FROM Worker W
JOIN Supervisor S ON W.SupervisorID = S.SupervisorID
WHERE S.Department = 'Tshirt';

SELECT *
FROM Worker
WHERE Department = 'Tshirt';




SELECT *
FROM Worker
WHERE Department = 'TShirt';


SELECT WorkerID, Name
FROM Worker
WHERE Department = 'TShirt';



SELECT *
FROM Workers
WHERE Department = 'Tshirt' AND Gender = 'Female';
SELECT *
FROM Worker
WHERE Department = 'Garments' AND Gender = 'Male';




SELECT * FROM Worker WHERE Gender = 'Female';



SELECT SUM(DailyOutput) as TotalOutput FROM Worker WHERE Gender = 'Female';





SELECT SUM(DailyOutput) as TotalMaleOutput FROM Worker WHERE Gender = 'Male';

SELECT * FROM Worker WHERE Plant = 'Plant1';



SELECT SUM(DailyOutput) as TotalOutput FROM Worker WHERE Plant = 'Plant1';




SELECT SUM(DailyOutput) as TotalOutput FROM Worker WHERE Plant = 'Plant2';



SELECT SUM(DailyOutput) as TotalOutput FROM Worker WHERE Plant = 'Plant3';




SELECT SUM(DailyOutput) as TotalOutput FROM Worker WHERE Plant = 'Plant4';




SELECT * FROM Worker WHERE Plant = 'Plant1';

SELECT * FROM Worker WHERE Plant = 'Plant2';

SELECT * FROM Worker WHERE Plant = 'Plant3';


SELECT * FROM Worker WHERE Plant = 'Plant4';

SELECT 
    (SELECT COUNT(*) FROM Worker WHERE Gender = 'Female') as FemaleWorkers,
    (SELECT COUNT(*) FROM Worker WHERE Gender = 'Male') as MaleWorkers,
    (SELECT COUNT(*) FROM Worker WHERE Gender = 'Female') / (SELECT COUNT(*) FROM Worker WHERE Gender = 'Male') as Ratio
;

