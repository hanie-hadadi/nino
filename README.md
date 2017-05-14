# Nino Services

Nino is a multiplatform system to create communication between children ( in kindergarten or school) and parents.



# Services

- Get Methods

| Service Name | Input | Output
| ------ | ------ | ------ |
| GetRooms |(string)sessionId, (int)pageNumber, (int)pageSize| EntityResultDto<list <room>>
| GetStudentsByRoomId |(string)sessionId, (int) roomId, (int)pageNumber, (int)pageSize|EntityResultDto<list <student>>
| GetAllStudentsByRoomId | (string)sessionId, (int)studentId, (int)pageNumber, (int)pageSize   | ServiceResultDto
| GetAllActivityType | (string)sessionId | EntityResultDto<list<<activityType>>>
| GetActivity | (string)sessionId, (int)activityId | EntityResultDto<activity>
| GetStudentActivity | (string)sessionId, (int)studentId, (int)pageNumber, (int)pageSize | EntityResultDto<activity>
| GetStudentActivityByType | (string)sessionId, (int)studentId, (string)ActivityType (int)pageNumber, (int)pageSize | EntityResultDto<activity>


- Add Methods

 Service Name | Input | Output
 | ------ | ------ | ------ |
 | AddRoom |(string sessionId, (string)name| EntityResultDto<room>
 | Addstudent |(string)sessionId, (string)name| id, name
 | AddStudentToRoom |(string)sessionId, (int)studentId, (int)roomId| ServiceResultDto
 | CheckInStudentToClass | (string)sessionId, (int)studentId, (int)classId  |  ServiceResultDto
 | CheckOutStudentFromClass | (string)sessionId, (int)studentId, (int)classId  |  ServiceResultDto
 |AddActivity | (string)sessionId,(array)Attributes  |  EntityResultDto<activity>

- Remove Methods

 Service Name | Input | Output
 | ------ | ------ | ------ |
 | RemoveRoom |(string) sessionId, (string)name| id, name
 | RemoveStudent |(string) sessionId, (string)name| id, name
 | RemoveStudentFromRoom |(string) sessionId, (int)studentId, (int)roomId| 


