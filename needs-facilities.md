# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given Separate entry and exit point is present for staff
  AND install the sensor at the entry and exit point on visitor gate
  When Visitor enters or exits the hospital through the visitor gate.
  Then Increment and decrement the count as per entry/ exit.

Scenario: Alert when seating capacity is full

  Given Place the Camera sensor at the seating area and install the alert system.
  When Threshold exceeds for occupied chair count.
  Then Alert the alert room to increase the seating space.
