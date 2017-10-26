# Project 4, Part 3 / C: Flickr and GitHub Collaboration

- Signup for `flickr` API key: https://www.flickr.com/services/api/
    - For this exercise, since we have provided the `cache_file.json`, you can put some random characters as `FLICKR_API_KEY`
- Create `config.py` based on `data/config_template.py`, and set the FLICKR_API_KEY
- Run `flickr.py`
- The output: "Mastering the dust by 126799981@N03" does not have the owner's username, but their ID number from Flickr's database
- Start a new development branch
- Modify the function `search_flickr_by_tags` to `search_flickr`, and make the code more general purpose, such that it can use (15 mins):
    - ```
        ...
        "method": "flickr.photos.search",
        "tags": tags,
        "per_page": 10,
        ...
      ```
    - and
    ```
        ...
        "method": "flickr.photos.getInfo",
        "photo_id": photo_id,
        ...
    ```
    - and other similar API calls
- Once 15 mins are up, commit and push to your fork whatever code you have in your development branch
- On github, create a pull request from your development branch into your master branch, but DON'T merge
- **Start a collaborative conversation with another person in the room, who is not sitting besides you**
    - Get their Github username
    - Mention them in your pull request's comments section on the lines of: "@anandpdoshi I have started modifying flickr_search function. Do you think I am on the right track? Can you see any flaws in it?"
    - You will answer to another person's request for help by reviewing their pull request at this stage
    - Using github, comment on at least 1 line of their code
    - Write a brief summary of your thoughts about their code in the pull request's comment thread
    - You can also exchange ideas about how to work on it
    - Similarly, you will get feedback on your own pull request
    - **DON'T close / merge this pull request**
- Use (or not) this feedback and continue writing code for `flickr_search`
- Load the owner's username into `owner_username` and update the `__str__` method to reflect that
- Once done, push your new changes to the same branch. Check your open pull request, and you will see that your new commits get added to the same pull request.
- Now you can ask for more feedback from your peer group if you want
- **Submit the link to this pull request as part 3 of Project 4**
