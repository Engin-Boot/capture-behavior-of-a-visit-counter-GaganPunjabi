# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given The computer system is running
  When Patient asks for appointment at registration desk
  Then Increment the patient count on successful registration

Scenario: Compute parking slots to reserve for visiting specialists

  Given Parking token is assigned to each vehical owner
  When Vehical enters the parking entry and ask for token
  Then Count number of tokens been assigned
