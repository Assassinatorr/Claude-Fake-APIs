# Claude-Fake-APIs
I recently brought a "cheap api" that is "from" claude, it has 500 credit only it and claims to be legit, only the issue is that its not, upon buying from a site they will tell you to go to powershell, 
connect to a different base url, use your bot to your hearts content, if you run out of credit to then buy more.... and harvest your data upon use whilst essentially getting complete system acces depending on you.

For example, in the image below i brought one to try it out and realised that its all fake, theres nothing legitimate about it on use.
<img width="330" height="187" alt="image" src="https://github.com/user-attachments/assets/e12abc99-1c21-4c3a-bccd-e6743b299001" />
Yes thats the real api key they gave me and the documentation to a fake claude site, 

# Enter these at your own risk
https://anthropic-api.com/docs
https://anthropic-api.com/merge
https://anthropic-api.com/ask

the key i got - sk-ant-api03-Db5av6SYi5Vz6lr4ppA2sAaQ2vzKmHVa1YOGl5YCvTPI6AcXyvX110-PzBz0oPZq6sETtDG2OetRQOYzD6xE3z-5RuDqN5x 
[THIS IS NOT A REAL CLAUDE API ITS A SCAM]
These are all FAKE

Essentially what you do it, you use a command to paste into powershell like the one below and they connect u to the claude network but its 10/10 times deepseek or another chinese ai model.

[System.Environment]::SetEnvironmentVariable("ANTHROPIC_BASE_URL", "[the fake site goes here so like] https://fakeapi.com", [System.EnvironmentVariableTarget]::User)
[System.Environment]::SetEnvironmentVariable("ANTHROPIC_AUTH_TOKEN", "YOUR API KEY", [System.EnvironmentVariableTarget]::User)

and then with your claude cli it would let you use different models [as if everything is legit] however you wish, the reason i caught on is due to the high error requests it kept sending back, over and over after a few lines it kept promting 400 and i
realised something was wrong.

They seem to have wrapped the key in a anthropic api and made it look identical but have then got flaws of error codes, and loads of other minor details.

Site of purchase - https://www.g2g.com/uk/categories/claude-ai-gift-cards
