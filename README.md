# data-VMo2-1705

Option 1:

- Connections thought Cloud SQL Auth Proxy
- Assigned roles/permissions and service accounts
- Access to Cloud SQL:
	- Segregation at Table level (assign privileges to users)
	- Row Security policies (pgsql feature that restrict on a per-user basis, which rows can be returned by normal queries or inserted, updated, or deleted by data modification commands)
	- Column level security (create user views/encrypt column data/column-level permissions)

Option 2:

- Cloud SQL date imported to BQ
- Add datasets permissions
- Restrict access at table level
- Create tag policy for columns
- Add row policy to the tables
