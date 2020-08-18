# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given Backup server is present
  When Primary server is not accessible
  Then Switch on the backup server and transfer the request to that server.

Scenario: Reconcile counts if the sensor is offline for a while

  Given A security guard is available.
  When Sensors are offline or non-functional
  Then Request is sent to the security guard to make the entry manually
