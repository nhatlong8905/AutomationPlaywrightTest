## Setup

1. To set up this project on your local machine, clone it from the GitHub repository.
2. From the command line in the project's root directory to install all dependencies by run:

   ```bash
   npm install
   ```

3. Next run the following command to download Playwright supported browsers:

   ```bash
   npx playwright install --with-deps
   ```

4. Finnaly run the following command to install cross environment:

   ```bash
   npm install -g cross-env
   ```

## Running Tests

From the command line in the project's root directory:

- Running the tests on PROD environment. By default tests will run without UI (headless mode):

```bash
   npm run test:prod
```

- You can also run the tests on PROD environment with UI (headed mode):

```bash
   npm run test:prod-headed
```

## Tests Output

- After the test finish. An output JSON file named `output.json` will be generated in the root directory. 

## Tests Report

All output file and report is stored in `./testOutput` folder. You can view both Allure and HTML report.

- Generate Allure report:

```bash
    npm run allure
```

- Show HTML test report:

```bash
   npx playwright show-report test-output/html
```
## Reference

- To show all Playwrigt option commnad :

```bash
   npx playwright --help
```
