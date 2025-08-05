### Create a custom authorization middleware
1. Create a folder "Entities" and populate it with how the DB will be 

** Create a static User to just test how thins will work: i.e
public class User{
	public string Username {get; set;} = string.Empty........
 }

 2. Create a folder "Models-- UserDto" for the DTO(Data transfer object)
	

3. Create the "authController" class in the controller folder


NB:For password hashing, normally, we can use bcrypt, but dotnet has an inbuilt function for that which is "ASP NET core Identity"(not the whole, we just need what we call "Hashser")


###### STEPS:
1. Create the register, login controller
2. Create the jwt token method that will be returned to the user
3. Now, Let's create the DB--

** a) create the dbContext file
	b) populate and set up the db Context for the "users"
	c) then register our database context in the program.cs

4. Now, after the dB integration, we create the SERVICE folder, service file and interface for service also
** a) we populate the service with our logics(registerAsync, loginAsync... etc)
   b) we then register our service in the program.cs also