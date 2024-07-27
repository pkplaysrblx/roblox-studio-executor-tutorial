# Tutorial on how to make an executor in Roblox Studio

Here are the steps.
 1. Make A ScreenGui in the StarterGui Folder
 2. Make a frame and name it and customise it to your liking.
 3. Make sure your gui has a execute button, clear button and the textbox to put your script in.
 4. Now in the execute button, create a local script and paste this code:
 5. ```
    yourbuttonname.MouseButton1Up:Connect(function()
	loadstring(Script.code)
	end)
    ```

 6. Now go into your clear button and paste this code in
   ```
   yourbuttonname.MouseButton1Up:Connect(function()
	Script.code = ''
	end)
   ```
 7. Lastly, paste this code into your textbox
    ```
    ExecuteButton.MouseButton1Click:Connect(function()
    local scriptCode = ScriptInput.Text
    local success, errorMessage = pcall(function()
        loadstring(scriptCode)()
    end)
    if not success then
        warn("Error executing script: " .. errorMessage)
    end
    end)
    ```
# Finished
You have now finished your script. You may execute it with your executor now!
If you are having issues, use the provided script and edit it.
    
