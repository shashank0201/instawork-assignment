# Instawork-assignment

Project

The goal of the project is to implement an HTTP API to support a team-member management
application. The team member data should be persisted in a MySQL database. The application
needs to support listing team members, adding a new team member, editing a team member,
and deleting a team member. The details are covered below.

### Listing team members
    This endpoint should return a JSON array of all team members in the application. For each team
    member, the following data should be included:
    ● a unique id
    ● first name
    ● last name
    ● phone number
    ● email
    ● role (this is either "admin" or "regular")

### Adding a team member
    - This endpoint should accept a JSON object in the body of the request.
    - The JSON object should include the same properties as above (first/last name, phone, email, role) except for the unique id. 
    - The API response should return a JSON object with the properties, including a unique id for the team member.

### Editing a team member
    - This endpoint should accept a JSON object in the body of the request. 
    - The JSON object can include any of the properties above (first/last name, phone, email, role).
    - The API response should return all of the (updated) properties of the team member.
    
    Note: Not all properties needs to be provided in the request. Properties that are not included
    should not be updated.

### Deleting a team member
    This endpoint should take a unique id for the team member and return an empty response.
    
### Notes
    ● The app should be implemented in Python using the Django web framework or NodeJS.
    The app should use a MySQL server as the database. All actions (creating, editing,
    deleting) should be persisted to the database.
    ● Do not build an HTML interface to show the data, only the API is required.
    ● You are allowed to use libraries to help build the app.
    ● Don't worry about multi-user cases or authentication. For this app, assume all clients see
    the same list of team members.
