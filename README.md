# Tutorial on how to make an executor in Roblox Studio

Here are the steps.
 1. Make A ScreenGui in the StarterGui Folder
 2. Make a frame and name it and customise it to your liking.
 3. Make sure your gui has a execute button, clear button and the textbox to put your script in.
 4. Now in the execute button, create a local script and paste this code:
 5. ```
    yourbuttonname.MouseButton1Up:Connect(function()
	loadstring(Script.code)
end)```

6.
