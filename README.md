import javax.swing.*;
public class Rectangle {
	private double width;
	private double height;

	public Rectangle() {
		this.width = 0;
		this.height = 0;
	}

	public Rectangle(double width, double height) {
		this.width = Math.abs(width);
		this.height = Math.abs(height);
	}

	public double getArea() {
		return width * height;
	}

	public double getWidth() {
		return this.width;
	}

	public void setWidth(double width) {
		this.width = Math.abs(width);
	}

	public double getHeight() {
		return this.height;
	}

	public void setHeight(double height) {
		this.height = Math.abs(height);
	}

}
public class RectangleDriver {
	public static void main(String[] args) {
		Rectangle rec = new Rectangle();
		System.out.println(rec.getArea());

		Rectangle rec1 = new Rectangle(1.2, 3.5);
		System.out.println(rec1.getArea());

		Rectangle rec2 = new Rectangle(-1.2, 3.5);
		System.out.println(rec2.getWidth() + " " + rec2.getHeight());

	}
}
