# try_selenium
## Selenium Python Web Automation

Python is a programming language that needs no introduction! It is one of the most preferred languages when it comes to projects involving Machine Learning (ML), Artificial Intelligence(AI), and more. On a different battleground, the combination of Selenium Python is widely preferred as far as website automation is concerned.

Selenium is an open-source tool that automates web browsers and it is the leader in its category. It can be executed in multiple browsers and operating systems, supporting several programming languages like C#, Java, Python, NodeJS. Selenium offers a suite of software responding to different testing needs.


## Interacting with the page

WebDriver offers a number of ways to find elements. For example, given an element defined as:
```
<input type="text" name="passwd" id="passwd-id" />
```
We can find elements in that way:
```
element = driver.find_element(By.ID, "passwd-id")
element = driver.find_element(By.NAME, "passwd")
element = driver.find_element(By.XPATH, "//input[@id='passwd-id']")
element = driver.find_element(By.CSS_SELECTOR, "input#passwd-id")
```
So, we’ve got an element. What can we do with it? First of all, we may want to enter some text into a text field:

```
element.send_keys("some text")
```
We can simulate pressing the arrow keys by using the “Keys” class:
```
element.send_keys(" and some", Keys.ARROW_DOWN)
```
We can simply clear the textarea field:
```
element.clear()
```
