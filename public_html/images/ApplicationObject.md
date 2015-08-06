A Application Object is used to Manipulate Data in the Application.

It wraps a View or a Data Object and holds Information about the edit state of the object,
and the chaged attributes.

Possible states are isNew, isChanged, isMarkedAsDeleted.




State Table

Server | Client | State (ClientView)
       |   1    | Created
    1  |   1    | Consistent
    1' |   1    | ChangendRemote
    1  |   1'   | Changed
   1*  |   1'   | Inconsistent
  (1)  |   1    | RemoteDeleted
   1   |  (1)   | MarkedAsDeleted
   1   |        | NotLoaded

  

 