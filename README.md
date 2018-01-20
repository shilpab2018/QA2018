# QA2018
Shilpa Bhowmick
attached file with xpath & method for the use case automation
Use Eclipse to run the code with help of selenium.WebDriver and selenium chromedriver import
Platform limitation - Maven is used as build automation tool.
Dependencies - Browser drivers, Selenium webdriver, Maven, Java
Code can be used for multi-browser automation given you have specific browser driver installed to use
Example when it's used to run in Chrome browser -
----------------------------------------------------------------------------------
import java.util.concurrent.TimeUnit;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class TestJob {

	public static void main(String[] args) throws InterruptedException {

		WebDriver driver;

		System.setProperty("webdriver.chrome.driver", "/Users/shilpa/chromedriver");

		driver = new ChromeDriver();

		driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);

		driver.get("http://www.qaworks.com/"); // url
    ---------------------------------------------------------------------------------
    
