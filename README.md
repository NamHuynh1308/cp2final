# cp2final
# 9/13/2021
_review about for loops
	+Ex: Pay attention to condition inside loop about the array length.
_Get some test on eclipse
import java.util.Arrays;

public class Aha {
    private String title;
    private int ISBN;
    private Integer[] values;
    
    public Aha(String title, int iSBN, Integer[] values) {
        this.title = title;
        ISBN = iSBN;
        this.values = values;
    }

    /**
     * @return the title
     */
    public String getTitle() {
        return title;
    }

    /**
     * @param title the title to set
     */
    public void setTitle(String title) {
        this.title = title;
    }

    /**
     * @return the iSBN
     */
    public int getISBN() {
        return ISBN;
    }

    /**
     * @param iSBN the iSBN to set
     */
    public void setISBN(int iSBN) {
        ISBN = iSBN;
    }

    /**
     * @return the values
     */
    public Integer[] getValues() {
        return values;
    }

    /**
     * @param values the values to set
     */
    public void setValues(Integer[] values) {
        this.values = values;
    }

    
    
    @Override
    public String toString() {
        return "Aha [title=" + title + ", ISBN=" + ISBN + ", values=" + Arrays.toString(values) + "]";
    }


# 9/15/2021
*Sharing data between classes
Another way to share data is inheritance.
_New class keyword: Extends
_New method/ data visibility keyword: protected
+This data item/ method is visible both inside the class and to classes that extend this class.
+Also visible to other classes in the same package
_UML 
Terminology
+Subclass: Child class
	Get direct access to all of the public and protected
+Superclass: Parent class, Base class => Product
Practise Modeling relationships
Ex: Shape: superclass
Ex2: Name: super class of first name, last name, middle name
**Inherited can be bad if done incorrectly
_Inherited is widely used in Java
*From one class
Public Aha( String title, ISBN, value) {
	This.title = title;
SetISBN(ISBN);
This.value = value
}
Public Aha() {
	Title = “what”
ISBN =9;
This.value = new Integer[999];
}

*From another class
Public class AAAAha extends Aha{
Public AAAAja() {
	//super();
}
Public static void main(String[] args) {
Var x = new AAAAha();
}
}
