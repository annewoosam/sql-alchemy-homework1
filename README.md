# sql-alchemy-homework1-  SYNTAX samples

Things to test after entering virtual env, creating database and loading models file interactively:

all_employees_nav()
all_employees_join()

(Note model.py createdb file will need to be comemnted out after first use)

cynthia = Employee.query.filter_by(name='Cynthia Dueltgen').one()

cynthia.dept

cynthia.dept.phone

db.session.query(Employee).filter(Employee.dept_code.is_(None)).all()

db.session.query(Employee.name).filter_by(fav_color='orange').all()

admin = Department.query.get('admin')
admin.emps

