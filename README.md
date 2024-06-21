# Running the application

`ddev start`

## Ingest the data

1. Copy DB back up file inside the DB container (OrbStack UI will be helpful to do this via getting a Finder session for DB container)
2. Run the command `mysql -u root db < drupal_backup_database.sql` (Same like above OrbStack UI will be helpful to get a terminal session for DB container)

## Notes

Any changes to settings, modules, contents will have to update the db backup.

How to get a back up:

1. Using OrbStack UI, initiate a terminal session for DB container, run below

`mysqldump -u root db > drupal_backup_database.sql`

2. Move this file to project root (OrbStack UI can be used to initiate a Finder session on DB container)
