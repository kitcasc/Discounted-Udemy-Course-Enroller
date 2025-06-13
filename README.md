<p align="center">
    <img src="https://raw.githubusercontent.com/techtanic/Discounted-Udemy-Course-Enroller/refs/heads/master/extra/promo.gif">
    <br/>
    <img src="https://forthebadge.com/images/badges/made-with-python.svg">
    <br/>
    <a href="https://github.com/techtanic/Discounted-Udemy-Course-Enroller/graphs/commit-activity"><img alt="Maintenance" src="https://img.shields.io/badge/Maintained%3F-yes-green.svg?style=for-the-badge"></a>
    <a target="_blank" href="https://discord.gg/wFsfhJh4Rh"><img alt="Discord" src="https://img.shields.io/discord/703266580846346361.svg?label=Discord&logo=Discord&colorB=7289da&style=for-the-badge"></a>
    <br/>
    <a href="https://github.com/techtanic/Discounted-Udemy-Course-Enroller"><img src="https://cdn.discordapp.com/attachments/823472016999972884/841661124410736710/standard_13.gif"></a>
</p>

# Discounted Udemy Course Enroller

> Software to enroll in available Udemy Paid/Free courses having coupons automatically to your Udemy account.

Everything you need can be on the website: https://techtanic.github.io/duce/

## Key Features

- Beautiful GUI
- One click login using Browser cookies.(Supports major browsers)
- One click to add all available courses with coupons to your udemy account
- Uses popular sites for coupons
- Many more features
- CLI version available for automation
- Advanced filters

# Downloads

<table>
<thead >
  <tr>
    <th style="text-align: center">GUI</th>
    <th style="text-align: center">CLI</th>
  </tr>
</thead>
<tbody>
  <tr align="center">
    <td><a href="https://github.com/techtanic/Discounted-Udemy-Course-Enroller/releases/latest/download/DUCE-GUI-windows.exe">
         <img alt="GUI Windows exe" src="https://img.shields.io/static/v1?message=Download&logo=windows&labelColor=5c5c5c&color=1182c3&label=%20&style=for-the-badge"
         >
      </a></td>
    <td><a href="https://github.com/techtanic/Discounted-Udemy-Course-Enroller/releases/latest/download/DUCE-CLI-windows.exe">
         <img alt="CLI Windows exe" src="https://img.shields.io/static/v1?message=Download&logo=windows&labelColor=5c5c5c&color=1182c3&label=%20&style=for-the-badge">
      </a></td>
    
  </tr>
</tbody>
</table>

<h2><details>
<summary>Screenshots of GUI</summary>

![Login](/extra/gui-login.png)

![Discounted Udemy Course Enroller](/extra/gui-main.png)

![Coupon Scraping](/extra/gui-scraping.png)

![Enrolling](/extra/gui-enrolling.png)

</details>

## Automated Execution with GitHub Actions

This repository includes a GitHub Actions workflow that automatically runs the script daily to enroll in free Udemy courses. Follow these steps to set up automated execution:

### Setup Instructions

1. **Fork this Repository**
   - Click the "Fork" button at the top right of this repository
   - This will create your own copy of the repository

2. **Enable GitHub Actions**
   - Go to your forked repository
   - Click on the "Actions" tab
   - If prompted, click "Enable Actions"
   - Ensure that Actions permissions are enabled in your repository settings:
     - Go to Settings > Actions > General
     - Under "Actions permissions", select "Allow all actions and reusable workflows"
     - Under "Workflow permissions", select "Read and write permissions"

3. **Configure Repository Secrets**
   - Go to your repository's Settings > Secrets and variables > Actions
   - Click "New repository secret"
   - Add the following required secrets:
     - `UDEMY_EMAIL`: Your Udemy account email
     - `UDEMY_PASSWORD`: Your Udemy account password
     - `BROWSER_COOKIES`: (Optional) Your browser cookies for automatic login
       - To get cookies, log in to Udemy in your browser
       - Use browser developer tools to copy cookies
       - Format: `name1=value1; name2=value2; ...`

4. **Verify Setup**
   - Go to the "Actions" tab
   - You should see a workflow named "Daily Course Enrollment"
   - The workflow will run automatically at 00:00 UTC daily
   - You can also manually trigger the workflow from the Actions tab

### Customization

- The workflow runs daily at 15:00 UTC by default
- You can modify the schedule in `.github/workflows/auto-enroll.yml`
- Choose what languages you want to enroll with `default-duce-cli-settings.json`
- The script uses the CLI version with default settings
- You can customize the script behavior by modifying the workflow file

### Troubleshooting

- Check the Actions tab for workflow run logs
- Ensure all required secrets are properly configured
- Verify that your Udemy credentials are correct
- If using cookies, make sure they are properly formatted and not expired

### Acknowledgments

This automated setup is based on the original project by [@techtanic](https://github.com/techtanic/Discounted-Udemy-Course-Enroller). Special thanks to the original creator for developing this amazing tool that helps people access free Udemy courses.

## Disclaimer

![](/extra/disclaimer.png)

## Donate

BTC `bc1qdyjwj0eqxjk5hxejah4gyclrumwtqs3hqp63uz`

BTC `14JNjiNoiKcbCHcxcqUxgJcVgyDfhGbxQF`


<center>
Made with ❤️
</center>