public class Pyramid {

    private String color;
    private   Rectangle rect;
    private double height;

    public Pyramid(String color,Rectangle rect,double height){                                    
        this.color=color;
        this.rect=rect;
        this.height=height;
    }

    public String getColor() { return color; }
    public double getRectangle() { return rect.getBase(); }
    public double getHeight() { return height; }
    //getters, setters
    public void setColor(String color) { this.color=color; }

    public void setHeight(double height) { this.height=height; }



    public void getVolume(){
        double volume=0;
        volume=rect.getBase()*height;
        volume/=3;
        System.out.println("pyramid's volume is= "+volume+" its color is= "+color);

    }
}
public class Rectangle {
    private double length;
    private double width;
    public Rectangle(double length,double width){                                    
        this.length=length;
        this.width=width;
    }
    public double getBase(){
        double base =length*width;
        return base;
    }

}
public class Test {

    public static void main(String[] args) {
        Rectangle b=new Rectangle(9,9);
     Pyramid a=new Pyramid("blue",b,1);
     a.getVolume();



    }
}

