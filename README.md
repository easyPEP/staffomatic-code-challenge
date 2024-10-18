# Staffomatic Code Challenge

This is a Ruby on Rails API code challenge for managing user schedules. Please follow the instructions below to complete the challenge and submit your work.

## Steps to Complete the Challenge

### 1. Create a New Repository

You will **not** clone or fork this repository directly. Instead, you should create a **new repository** from this one using a mirror. This ensures there are no links between your repository and the original.

#### Mirror the Repository

1. Clone the repository as a bare repository:

   ```bash
   git clone --bare https://github.com/easyPEP/staffomatic-code-challenge staffomatic-code-challenge
   ```

2. Create a new repository on your GitHub account (e.g., `staffomatic-code-challenge`), but **do not initialize** it with a README, license, or `.gitignore`.

3. Mirror-push the bare repository to your new repository:

   ```bash
   cd staffomatic-code-challenge
   git push --mirror https://github.com/[YOUR_USERNAME]/staffomatic-code-challenge.git
   ```

4. Remove the temporary local mirror repository:
   ```bash
   cd ..
   rm -rf staffomatic-code-challenge
   ```
5. Clone the new repository to your local machine:

   ```bash
   git clone https://github.com/fluxsaas/staffomatic-code-challenge.git staffomatic-code-challenge
   cd staffomatic-code-challenge
   bundle install
   echo "ebeb5c739426e455d429f3d011384b77" > config/master.key
   ```

6. Run Specs or server:

to run the server:

```bash
bin/setup
```

to run the specs with guard:

```bash
guard
```

Now, you should have a **new repository** on your GitHub account without any connection to the original repository.

### 2. Create a Feature Branch

Once the repository is mirrored, create a new branch (e.g., `feature/user-allocation`) to work on your solution:

```bash
git checkout -b feature/user-allocation
```

### 3. Make Your Changes

Proceed to implement the required features, tests, and configurations for the challenge, following the provided specifications.

### 4. Create a Pull Request (PR)

Once your changes are complete:

1. Push your changes to your remote repository:

   ```bash
   git push origin feature/user-allocation
   ```

2. Create a pull request (PR) from your feature branch (`feature/user-allocation`) to the `develop` branch in **your repository**.

### 5. Invite for Code Review

After creating the PR, invite me (`[your GitHub username]`) as a collaborator on your repository. You can do this by going to your repository's **Settings** → **Manage Access** → **Invite Collaborator**.

Please leave a note on the PR inviting me to review the work.

---

## Other Instructions

- Follow the setup, testing, and deployment instructions outlined in the sections above to ensure the app works correctly.
- Ensure your code is well-documented and that all tests pass.
- Use best practices for code design, and ensure that the app is easily extendable for future modifications (e.g., adding new `source_type`).
