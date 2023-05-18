# DoctorApp 👋

## Frameworks and Language used:
 - Spring
 - Spring boot
 - My-Sql
 - Java


 ## Data Flow
 #### Controller
---Appointment----
 - bookAppointment
 - doctor
 - patient

 ---Doctor----
 - addDoctors
 - getDocMyAppointments
 - updateOrder

 ---Patient----
 - signUp
 - signIn
 - getAllDoctors
 - cancelAppointment

 #### Service
  ---Appointment----
 - bookAppointment
 - cancelAppointment

 ---Authentication----
 - saveToken
 - getToken
 - authenticate

 ---Doctor----
 - addDoc
 - getAllDoctors
 - getMyAppointments

 ---IAuth----
 - saveToken
 - getToken
 - authenticate

 ---Patient----
 - signUp
 - encryptPassword
 - signIn
 - getAllDoctors

 #### Repository
 ---Appointment----

 IAppointmentRepo

 ---Doctor----

 IDoctorRepo

 ---Patient----

 IPatientRepo

 ---Token----

 ITokenRepo

 #### Model
 ---Appointment----
 - id
 - doctor
 - patient
 
 ---AppointmentKey----
 - appId
 - time

 ---AuthenticationToken----
 - tokenId
 - token
 - tokenCreationDate
 - patient

 ---Doctor----
 - doctorId
 - doctorName
 - specialization
 - appointment

---Patient----
- patientId
- patientFirstName
- patientLastName
- patientEmail
- patientPassword
- patientContact

#### dto
 ---SignInInput----
 - patientEmail
 - patientPassword
 
 ---SignInOutput----
 - status
 - token

 ---SignUpInput----
 - userFirstName
 - userLastName
 - userEmail
 - userPassword
 - userContact

 ---SignUpOutput----
 - status
 - message
 
### Project Summary
Created a simple Doctor Application which doctor,patient and appointment as model to provide differnet CRUD operations like:-
addDoctor,bookApoointment,cancelAppointment etc.This application provides the basic functionality of a doctor patient management system.

### How to use in your system?
 - Just Simply clone this reposit
 - Start your server
 - Perform operations 
