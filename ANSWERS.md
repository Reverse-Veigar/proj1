# Q0: Why is this error being thrown?
We have not yet made the Pokemon model.

# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
Random trainerless Pokemon are being selected via the index method in the Home controller. Any trainerless pokemon can appear from the database.

# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.
This line creates a clickable button on the home page that sends a patch request with the capture_path containing the current wild pokemon's id. The patch request will bind the pokemon to the current trainer's id making it theirs.

# Question 3: What would you name your own Pokemon?
JaxJax

# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
I passed a path trainers/:id into the redirect_to but it needs the id of the trainer we wish to look at so that the proper page shows.

# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
In application.html.erb, at the end of the file it has render 'layout/messages' so any validations that error will be displayed as sentences.

# Give us feedback on the project and decal below!
Overall ok but alot of problems for people with Windows as numerous errors caused confusion.

# Extra credit: Link your Heroku deployed app
