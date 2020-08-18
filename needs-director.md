# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given The computer system is running
  When Patient asks for an appointment at the registration desk
  Then Increment the patient count on successful registration

Scenario: Compute parking slots to reserve for visiting specialists

  Given Record the Schedule of Specialists visiting the hospital.
  When Vehicle enters the parking entry and asks for a patient token
  Then Assign tokens if the space is available.
