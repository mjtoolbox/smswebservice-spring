WebService
FindAll: http://localhost:8080/smswebservice-spring/spring/students
FindByID: http://localhost:8080/smswebservice-spring/spring/students/1001

HTML
http://localhost:8080/smswebservice-spring/index.html


JSON import in MongoDB
New command prompt and type below
>  mongoimport -d test -c students --file "c:/devapps/mongodb/students.json"


> db.students.ensureIndex({id:1},{unique:true})
(create an index on "id" field, which needs to be unique)

> db.sequence.insert({_id: "studentid", seq: 1007})
(Create a new collection calls "sequence" and insert one number)

> db.getCollectionNames()
[ "sequence", "students", "system.indexes" ]

