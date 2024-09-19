System.out.println(( emplist.get(i)).getClass().getName()); giving type cast error


The issue you're encountering is likely because emplist.get(i) is not of the expected type when you're trying to access or print its class name. To resolve this, here are a few steps to check:

Ensure the type of elements in emplist: Make sure that emplist is of a generic type, such as List<Employee> or ArrayList<Employee>. If you're using a raw list (e.g., ArrayList without a type parameter), you may run into casting issues.

List<Employee> emplist = new ArrayList<>();

Check if elements in emplist are of a consistent type: If you're mixing types in emplist, for example, adding objects of different types (not just Employee objects), this could lead to issues when casting or calling getClass().

Proper type casting: If you're using a raw ArrayList or List, make sure to cast the object to the correct type before calling methods on it. Here's how you could cast the object to the correct type before calling getClass():

System.out.println(((Employee) emplist.get(i)).getClass().getName());

Use Generics: If you're using generics correctly, there shouldn't be a need for explicit casting. Here is an example with generics:

List<Employee> emplist = new ArrayList<>();
System.out.println(emplist.get(i).getClass().getName());
