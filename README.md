# MVC Model, View, Controller

## What is MVC?
MVC stands for Model, View, Controller. It's a way of organizing your code so tha each particular section of your code performs a similar function.

- Model
    - Model is the layer that is responsible for connection your database. A model is a reperesentation one or more records from table in your database.

class User  -> extends Model -> uses Database class -> uses PDO class -> to query your MySQL database
class Project -> extends Model -> uses Database class -> uses PDO class -> to query your MySQL database


class Model
{
    $table = '';

    // ... all functionailty to query database
}

class User 
{
 $table = 'users';
}

- View
   - A View is the UI/ display that we show the user. It could HTML, JSON, XML, etc., but it should not contain any logic related to anyting expcept presentation. (looping over things to display in a list, etc.)

   - Controller
     -Controller is the connecting piece between your Views and your Models. It's the layer where all your "business logic" live; meaning any logic that isn't reallt catagorize into database / data storage, or presentation.# week-6
