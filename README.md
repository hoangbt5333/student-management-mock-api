## Student Management Mock API

Start the API from this directory:

```bash
npm install
npm start
```

JSON Server listens on `http://localhost:3001`. Port 3000 may already be used by another local service.

Collections in `db.json`:

- `/students`: student records; class relation uses `classId`.
- `/classes`: classes.
- `/teachers`: teacher records.
- `/subjects`: subjects; optional teacher relation uses `teacherId`.
- `/grades`: score records; relations use `studentId` and `subjectId`.

JSON Server provides GET, POST, PUT/PATCH and DELETE for these collections. Grades are limited by the Angular form to 0–10; the mock API itself does not enforce that rule.