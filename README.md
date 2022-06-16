import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.interactions.Actions;


public class Filter{

public static void main(String[] args) {
  WebDriver driver = new ChromeDriver();
  driver.get("http://www.flipkart.com/");
  driver.manage().window().maximize();
  // Login to the flipkart:
  webElemnet Username=driver.findElement(By.xpath("/html/body/div[2]/div/div/div/div/div[2]/div/form/div[1]/input").sendkeys("sakthivelparthiban25@gmail.com");
  webElemnet Password=driver.findElement(By.xpath("/html/body/div[2]/div/div/div/div/div[2]/div/form/div[2]/input").sendkeys("sakthivel@123");
  webElemnet loginbtn=driver.findElement(By.xpath("/html/body/div[2]/div/div/div/div/div[2]/div/form/div[4]/button").click();
  // Search the watch:
  webElemnet searchicon=driver.findElement(By.xpath("//*[@id="container"]/div/div[1]/div[1]/div[2]/div[2]/form/div/button/svg").sendkeys("watch");
  //Filter the watch
   
  Actions act = new Actions(driver);
  //select minimum amount
  WebElement min = driver.findElement(By.xpath("//*[@id="container"]/div/div[3]/div[1]/div[1]/div/div[1]/div/section[2]/div[4]/div[1]/select"));
  act.moveToElement(min).build().perform();
  Select mindropdown = new Select(min));  
  mindropdown.selectByIndex(2);  
  WebElement max = driver.findElement(By.xpath("//*[@id="container"]/div/div[3]/div[1]/div[1]/div/div[1]/div/section[2]/div[4]/div[3]/select"));
  act.moveToElement(max).build().perform();
  Select mindropdown = new Select(max));  
  mindropdown.selectByIndex(3);  
  //brand search 
  WebElement brandsearchbar=driver.findElement(By.xpath("//*[@id="container"]/div/div[3]/div[1]/div[1]/div/div[1]/div/section[3]/div[2]/div[1]/div[1]/input").sendkeys("titan");
  driver.findElement(By.xpath("//*[@id="container"]/div/div[3]/div[1]/div[1]/div/div[1]/div/section[5]/div[2]/div[1]/div[2]/div/label/div[2]")).click();
  //ideal for checkbox
  driver.findElement(By.xpath("//*[@id="container"]/div/div[3]/div[1]/div[1]/div/div[1]/div/section[6]/div[2]/div/div[3]/div/label/div[2]")).click();
  driver.manage().timeouts().implicitlyWait(30, TimeUnit.5000); 
  //Discount offer checkbox
 driver.findElement(By.xpath("//*[@id="container"]/div/div[3]/div[1]/div[1]/div/div[1]/div/section[7]/div[2]/div/div[5]/div/label/div[2]")).click();
 driver.manage().timeouts().implicitlyWait(30, TimeUnit.5000); 
 //customer rating
 driver.findElement(By.xpath("//*[@id="container"]/div/div[3]/div[1]/div[1]/div/div[1]/div/section[16]/div[2]/div/div[1]/div/label")).click();
  driver.manage().timeouts().implicitlyWait(30, TimeUnit.5000); 
  driver.close();
}}
