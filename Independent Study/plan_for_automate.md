This is a quick step-by-step barebone description of the possible plan for intergrating `automate` (this what we are calling the automated scheduling feature atm) to GTHC

- Review ruby code
  - Mike Olsen re-wrote his gScript code for his Google Sheets addon to ruby. I (Aman) will review and test that his code does what it is intended to do. This may require reaching out to Mike and working with him on getting any fixes.
- Create the ruby gem
  - Once the code is working properly locally, we will format it to work as a ruby gem and port it to the Ruby Gem repository for mass use.
  - This was decided to be the best choice so that the algorithm does not need to be forced upon the web app and they can be updated seperately.
- Add ruby gem to GTHC
  - Use this gem in API calls 
- Integrate new API endpoint data to frontend
  - Take this changed data and have it displayed for users in the proper manner
