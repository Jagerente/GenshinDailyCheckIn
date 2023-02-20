# Genshin Daily Check-In

This GitHub repository includes a workflow that automatically sends a daily curl request using your confidential credentials, which are securely stored in your forked repository. This ensures that the project runs smoothly and maintains its intended functionality.

To ensure proper functioning, please remember to update your credentials every time you log back into your https://www.hoyolab.com/ account as the ltoken refreshes with each login. This will help maintain the integrity of the account and ensure that the necessary authentication tokens are up-to-date.

![paimon](https://media.tenor.com/vlJ_b9xSgUQAAAAi/paimon-food-paimon-ehe.gif)

## Instructions:

1. Fork this repository.
2. Sign in to https://www.hoyolab.com/ and open the developer tools. Find the UID and token by navigating to F12 > Application > Cookies > https://www.hoyolab.com. The values are `ltoken` and `ltuid`, there may be multiple instances of each, so take any of them.

![devtools](https://user-images.githubusercontent.com/47350537/220109882-edc2f62b-c30f-47b1-9f23-d474fb08e8b3.png)

4. Set up secrets for the automatic workflow by navigating to Settings > Secrets and Variables > Actions > New Repository Secret. The names of the secrets must be TOKEN for `ltoken` and UID for `ltuid`. 

![secrets](https://user-images.githubusercontent.com/47350537/220113101-d4d4b3be-27cc-440c-8e95-0fd588145fb2.png)

5. You are done! Check status at Actions tab in your forked repository.

![actions](https://user-images.githubusercontent.com/47350537/220111084-bbd25613-ee99-4c5e-986e-55e45037116e.png)
