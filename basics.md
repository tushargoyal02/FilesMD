# NAVIGATION COMMANDS


*   GOING BACK TO THE BACK PAGE

    *   driver.back()

*   to front PAGE
    *   driver.forward()

*   To delete whatever you typed
    *   driver.send_keys(Keys.RETURN)

 *  To refresh the page
    *   driver.refresh()

*   Get browser version
    *   print(driver.capabilities['version'])

*   Get current url 
    *   print(driver.current_url)

*   Open a new tab for the keys you send or keys you find

        driver.send_keys(Keys.CONTROL + 't')


### Setting the window size

*   Set any size
    *   driver.set_window_size(1024,768)
*   To maximize window
    *   driver.maximize_window()

