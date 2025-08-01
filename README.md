# oop

package sample;
public class Book{
	String title;
	String author;
	int bookCount=0;
	final int bookID;
	static {
		int bookCounter=1000;
		final String LIBRARY_NAME="Central Library";
	}
    Book(){
    	this.title="Default Title";
    	this.author="Default Author";
    }
    public void Book(String title,String author) {
    	this.title=title;
    	this.author=author;
    	bookCount++;
    	bookId=bookCounter-1;
    }
    public void displayInfo() {
    	System.out.println("Title: "+title);
    	System.out.println("Author: "+author);
    }
    public void displayInfo(boolean showLibrary){
    	if(showLibrary==true) {
    		System.out.println(LIBRARY_NAME);
    	}
    }
    public void displayTotalBooks(){
    	System.out.println("Total number of books: "+bookCount);
    }
}
public class Main1 {
	Book b1=new Book();
	Book b2=new Book();
	Book b3=new Book();
	Book b4=new Book("How to be a good ");
	Book b5=new Book();
	Book b6=new Book();
}
