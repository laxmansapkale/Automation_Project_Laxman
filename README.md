# Automation_Project_Laxman
#THIS PROJECT IS CREATED FOR OUR WORK


package pom_fb;

import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.support.FindBy;
import org.openqa.selenium.support.PageFactory;

public class loginpom {
	
	//Declaration
	
	@FindBy(xpath="//input[@name='email']") private WebElement UserId;
	@FindBy(xpath="//input[@name='pass']") private WebElement Pass;
	@FindBy(xpath="//button[@name='login']") private WebElement Loginbutton;
	@FindBy(xpath="//button[@name='login']") private WebElement Creatbutton;
	@FindBy(xpath="//button[@name='login']") private WebElement Forrgotbutton;
	
	
	loginpom(WebDriver driver){
		
		PageFactory.initElements(driver, this);
	}
	
	//usage
	public void Enteruserid(String laxmansapkale) {
		UserId.sendKeys(laxmansapkale);
	}
	
	public void Enterpassword(String password) {
		Pass.sendKeys(password);
	}
	
	public void EnterLoginButton() {
		
		Loginbutton.click();
	}
	
}
