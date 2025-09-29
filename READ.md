A) INNER JOIN - Users who have at least one role
Returns only users who have at least one assigned role, combining user info with their role(s). Users without roles are excluded.

B) LEFT JOIN - All users (with profile info if present)
Returns all users, including those without profiles. If a user doesn’t have a profile, the profile columns show NULL.

C) RIGHT JOIN - Keep all roles even if unassigned
Returns all roles, including those not assigned to any user. Users without roles appear as NULL.

D) FULL OUTER JOIN 
Emulates a FULL OUTER JOIN in MySQL, showing all users and all profiles, even if some users don’t have profiles and some profiles don’t have matching users.

E) CROSS JOIN - 
Returns all possible combinations of users and roles. Each user is paired with every role regardless of assignments.

F) SELF JOIN - 
Shows referral relationships by joining the users table to itself via the referrals table, listing who referred whom and when.

G) Bonus - 
Shows each user’s latest login if available. Users who never logged in still appear with NULL login info.
