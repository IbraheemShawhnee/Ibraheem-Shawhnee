# Ibraheem-Shawhnee
![visitors](https://visitor-badge.glitch.me/badge?page_id=page.id)
<img height="180em" src="https://github-readme-stats.vercel.app/api?username=Gapur&show_icons=true&hide_border=true&&count_private=true&include_all_commits=true" />
name: Waka Readme

on:
  workflow_dispatch:
  schedule:
    # Runs at 12am UTC
    - cron: "0 0 * * *"

jobs:
  update-readme:
    name: Update this repo's README
    runs-on: ubuntu-latest
    steps:
      - uses: athul/waka-readme@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
