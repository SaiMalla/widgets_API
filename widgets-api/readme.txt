I developed an API which consists the functionality of the user signup, login and managing their TODO widget.

Pre-requisites:

ruby version >=2.2.2 
rails version 5


API Endponts:

    Prefix Verb   URI Pattern                         Controller#Action
auth_login POST   /auth/login(.:format)               authentication#authenticate
    signup POST   /signup(.:format)                   users#create
todo_items GET    /todos/:todo_id/items(.:format)     items#index
           POST   /todos/:todo_id/items(.:format)     items#create
 todo_item GET    /todos/:todo_id/items/:id(.:format) items#show
           PATCH  /todos/:todo_id/items/:id(.:format) items#update
           PUT    /todos/:todo_id/items/:id(.:format) items#update
           DELETE /todos/:todo_id/items/:id(.:format) items#destroy
     todos GET    /todos(.:format)                    todos#index
           POST   /todos(.:format)                    todos#create
      todo GET    /todos/:id(.:format)                todos#show
           PATCH  /todos/:id(.:format)                todos#update
           PUT    /todos/:id(.:format)                todos#update
           DELETE /todos/:id(.:format)                todos#destroy

 
Dependency gems for testing:


•	rspec-rails - Testing framework.
•	factory_bot_rails - A fixtures replacement with a more straightforward syntax.
•	shoulda_matchers - Provides RSpec with additional matchers.
•	database_cleaner - It cleans our test database.
•	faker - Library for generating fake data. 


Command to run the tests:


bundle exec rspec


