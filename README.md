public class Library {
public static void main(String[] args) {
System.out.println("*~Library~*")
System.out.println("Enter 1 to add a book || Enter 2 to remove a book || Enter 3 to Exit Library");
Scanner inpvalue = new Scanner(System.in);
int var = inpvalue.nextInt();
if(var == 1) {
System.out.println("Enter book title");
Scanner inp_val = new Scanner(System.in);
String book_title = inp_val.nextLine();

System.out.println("Enter author\'s name");
String book_author = inp_val.nextLine();


System.out.println("Enter no of pages");
String book_pgs = inp_val.nextInt();

Edit.Add(bookPage, book_title, book_author, book_pgs);
}

else if(var == 2) {
System.out.println("Enter book title to remove");
Scanner inp_val = new Scanner(System.in);
String book_title = inp_val.nextLine();
Edit.Remove(bookPage, book_title);
}

else if(var == 3) {
return;
}

else {
System.out.println("! Entered choice does not exist !");
return;
}
}