# praktika2ikbo16-17
Сделать форк, написать ФИО, группу. Приложить файлы реализации задания 
# Гарянин Никита Андреевич , ИКБО-16-17
# Author.java
<pre>
import java.lang.*;
public class Author
{
    private  String name;
    private String  email;
    private char gender;
    public Author(String name, String email, char gender)
    {
        this.name = name;
        this.email = email;
        //this.gender = gender;
        if (gender == 'M')
        {
            this.gender = 'M';
        }
        else if (gender == 'F')
        {
            this.gender = 'F';
        }
            else
            {
                this.gender = 'U';
            }
    }
    public String getName()
    {
        return name;
    }
    public String getEmail()
    {
        return email;
    }
    public char getGender()
    {
        return gender;
    }
    public void setEmail(String email)
    {
        this.email = email;
    }
    @Override
    public String toString()
    {
        return "Author: " + getName() + " gender: " + getGender() + " Email: " + getEmail();
    }
    }
</pre>

# TestAuthor.java
<pre>
public class TestAuthor
{
    public static void main(String[] args) {
        Author  author = new Author("Author1","123546@m.r",'y');
        System.out.println(author.toString());
        Author  author2 = new Author("Author2","12354m.r",'M');
        System.out.println(author2.toString());
        Author  author3 = new Author("Author3","1246@m.r",'F');
        System.out.println(author3.toString());
    }
}
</pre>
