-- Users Table
INSERT INTO users (user_id, username, password_hash, role) VALUES
(1, 'admin', 'hashedpassword123', 'admin'),
(2, 'faculty1', 'hashedpassword123', 'faculty'),
(3, 'student1', 'hashedpassword123', 'student');

-- Students Table
INSERT INTO students (student_id, name, email, phone, user_id) VALUES
(1, 'John Doe', 'john.doe@example.com', '123-456-7890', 3);

-- Faculty Table
INSERT INTO faculty (faculty_id, name, department, email, user_id) VALUES
(1, 'Dr. Smith', 'Computer Science', 'dr.smith@university.com', 2);

-- Courses Table
INSERT INTO courses (course_id, name, code, faculty_id, schedule) VALUES
(1, 'Java Programming', 'CS101', 1, 'MWF 10:00-11:00');

-- Enrollments Table
INSERT INTO enrollments (enrollment_id, student_id, course_id) VALUES
(1, 1, 1);
