# Library management system

## Class

### Users

--- Users are all people who have access to the library platform ---

**Instance Variables:**

* Name
* Mail address  
* Nationality
* password

**Method in the supervisor class:**

---
1. Login
---

This method allow any user to login in his/her account and start using the library based on who he is (Student, Facilitator or Supervisor).

---
2. Log out
---
This method allow any user to log out of the account.

---
3. Register
---

This method allow any user to be part of the ALU library system

#### Supervisor (Child Class of Users):

--- the supervisor is the person in charge of the library ---
--- We can have more than one supervisors---

**Instance Variables:**

* Name
* Mail address  
* Nationality
* password

**Method in the supervisor class:**

---
1. Add Book
---

This method gives the supervisor the possibility to add a book in the book collection.
It should return nothing.  

---
2. Remove Book:
---

This method gives the supervisor the possibility to remove a book in the Library.

---
3. See status of the library
---

This method allow the Supervisor to see the status all books.
This method returns the address of students who have not yet return books and the who still have the book after the required time.

#### Students (Child Class of Users):

*Instance Variables:*

* Name
* Mail address  
* Nationality
* Student ID
* Number of Book
* password

**Method in the Student's class:**

---
1. Borrow Book
---

This Method allow the student to borrow a book from the library for a short period of time.
The method returns the name of the book and the ID of the book.

---
2. Return Book
---

This method allow the user to return the book back in the library before exceeding the amount of time the student asked for.


#### Facilitator (Child Class of Users):

**Instance Variables:**

* Name
* Mail address  
* Nationality
* Student ID
* password

**Method For Facilitator**

---
1. Borrow Book
---

This Method allow the student to borrow a book from the library for a long period of time.
This same method allow the user to borrow books and hand it over to the students.
The method returns the name of the book and the ID of the book.

---
2. Return Book
---

This method allow the user to return the book back in the library before exceeding the amount of time the student asked for.


### Books :

*Instance Variables:*

* Book ID
* Book Name
* Published Date
* Acquisition Date
* Category
* Status

#### Paper Book(Child Class of Books):

**Instance Variables:**

* Cite bought
* Number of pages

**Method of the Paper book's class:**

---
1. Add Paper Book
---

This method receive instruction from the method called by the supervisor (Add book) and add the book to the list of Paper books.

---
2. Remove paper book
---

This method receive instruction from the method called by the supervisor (Remove book) and then remove the book to the list of Paper books.


#### Digital book(Child Class of Users):

**Instance Variables:**

* Cite bought
* Size of the book
* Google Drive Link

**Method of the Digital book's class:**

---
1. Add Paper Book
---

This method receive instruction from the method called by the supervisor (Add book) and add the book to the list of Digital books.

---
2. Remove paper book
---

This method receive instruction from the method called by the supervisor (Remove book) and then remove the book to the list of Digital books.
