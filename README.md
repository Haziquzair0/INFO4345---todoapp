Laravel CRUD Application with Profile Management

This Laravel project is a CRUD application enhanced with user profile management functionality. Below is a summary of the enhancements made to the project, including modifications to the Model, View, and Controller (MVC) components.

Enhancements

1. Profile Management
- Added functionality for users to update their profile information, including:
  - Nickname
  - Avatar (profile picture)
  - Email
  - Password
  - Phone Number
  - City
- Added functionality for users to delete their account, including removing their avatar from storage.

2. Registration Page
- Enhanced the registration page to include additional fields:
  - Nickname
  - Avatar (profile picture upload)
  - Phone Number
  - City
- Updated the `RegisterController` to handle these new fields and save them to the database.


Modified Files

1. Model
`app\Models\User.php`
- Added the following fields to the `$fillable` array to allow mass assignment:
  ```php
  protected $fillable = [
      'name', 'email', 'password', 'nickname', 'avatar', 'phone_no', 'city',
  ];
