# puppeteer
program for navigating through https://www.google.com/ using puppeteer
const puppeteer = require('puppeteer');
puppeteer.launch().then(async browser => {
  const page = await browser.newPage();
  await page.setViewport({ width: 1280, height: 800 })
  await page.goto('https://www.google.com/');
  await browser.close();
});
