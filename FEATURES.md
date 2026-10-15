# FEATURES

Update with every commit. Put a status (in-progress) or (complete) at the end of each line that you work on.

# Step 1: Report failures
* 1.1 Page keeps a list of error messages in state and shows them below the table
* 1.2 failed add, change, or delete adds a message saying what failed
* 1.3 starting any add, change, or delete clears the messages

# Step 2: Move section state up to Course
* 2.1 fix: deleting a section while another is being added no longer brings the deleted one back
* 2.2 Course keeps each section's data and status (pending or not) in its list
* 2.3 Section has no state, it displays what Course passes it
* 2.4 Course has the change instructor handler, passed down to each Section as a prop
* 2.5 the Pending overlay shows on a section while its change or delete is waiting

# Step 3: Add Section
* 3.1 the new section appears immediately, pending until the server confirms
* 3.2 the Add Section select goes back to "Add Section..." immediately, ready for another add
* 3.3 if the server fails, the new section is removed

# Step 4: Change Section
* 4.1 the select shows the new instructor immediately, pending until the server confirms
* 4.2 if the server fails, the select goes back to the previous instructor

# Step 5: Delete Section
* 5.1 the section stays, pending, until the server confirms the delete
* 5.2 if the server fails, the section stays
