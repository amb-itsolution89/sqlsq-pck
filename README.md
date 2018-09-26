The solution provides a mechanism generating Siebel sequences and inserts the generated sequence in the table in the target database for new created records.
For every record, requiring the sequence, the mechanism generates this sequence, and the sequence can be populated when the record is inserted into the target table in the database

Postgres is used to control the sequence increment. The increment works from 1 up to 100. Once is completed, the Postgres sequence is restarted and another bulk of sequence is generated with the incremental value from Postgres.
