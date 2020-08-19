# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given Add all entries manually in personal computer
  When Server is not running.
  Then Start Synchronization program to add all entries in a personal computer to the server

Scenario: Reconcile counts if the sensor is offline for a while

  Given A security guard is available.
  When Sensors are offline or non-functional
  Then Send request to the security guard to make the entry manually
