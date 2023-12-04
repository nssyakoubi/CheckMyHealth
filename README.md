# CheckMyHealth
I wouls like to add a new file to learn 
package JqueryUiHomework;

import java.time.Duration;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.annotations.Test;


public class Jquery {
	

	private WebDriver driver; // variable driver
	private String websiteURL = "https://jqueryui.com/draggable/";
	@Test
	public void StartJquery()  {
		try {

			// System.setProperty("webdriver.chrome.driver",
						// "src\\test\\resources\\drivers\\chromedriver.exe");
					// start chrome driver 
					System.out.println(" Step1 : opening the chrom driver");
					driver = new ChromeDriver();
					driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(30));
					driver.manage().timeouts().pageLoadTimeout(Duration.ofSeconds(30));
					driver.manage().window().maximize();
					driver.get(websiteURL);   //Get the website title 
					driver.getTitle();
					Thread.sleep(5 * 1000);
					
					// navigate to mortgage calculate website 
					// Get Website title and verify if WebTitle is matching with expected webTitle
					System.out.println(" Step2 : go to website :" + websiteURL);
					driver.get(websiteURL);   //Get the website title 
					driver.getTitle();
					
