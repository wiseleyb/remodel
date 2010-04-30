1. .all wasn't working - possibly added some inefficiency here.
2. added a default .to_s to the Entity object that returns id.to_s - this helps rails routing paths work
3. added this to find - since by default all finds in rails are string ids... key = key.to_i if key.to_i.to_s == key
4. added auto support for created_at and updated_at
5. added support for new_record?
6. fixed .all issue (missing *)