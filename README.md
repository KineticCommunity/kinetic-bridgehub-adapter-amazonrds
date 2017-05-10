# kinetic-bridgehub-adapter-amazonrds
A Kinetic Bridgehub adapter for Amazon RDS

Structures
**
Fields

* MonitoringRoleArn, InstanceCreateTime, DbiResourceId, PreferredBackupWindow, MonitoringInterval, DBInstanceArn, LatestRestorableTime, Engine, LicenseModel, EngineVersion, StorageType, DBInstanceStatus, DBInstanceClass, AvailabilityZone, PreferredMaintenanceWindow, ReadReplicaDBInstanceIdentifiers, DBInstanceIdentifier, CACertificateIdentifier, PendingModifiedValues, DBSecurityGroups, MasterUsername, DBName, DomainMemberships, SecondaryAvailabilityZone, EnhancedMonitoringResourceArn
Queries

Amazon RDS has a plethora of query parameters that can be passed in to filter your search.
Examples can be found at http://docs.aws.amazon.com/AmazonRDS/latest/APIReference/API_DescribeDBInstances.html

Methods:

Count: returns a count of DBInstances for the given user based on credentials.  Takes no structure or qualifications.

Return: qualification is DBInstanceIdentifier={DBInstanceIdentifier} | field is one or more of fields i.e.:  Fields: FreeStorageSpace | Qualifications: Dimensions.member.1.Value={DBInstanceIdentifier}


Search: returns list of instances by field (available fields listed above in fields).  Note: include DBName in fields in order to see name of each DB for the corresponding fields being searched for.  
