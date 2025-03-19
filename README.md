Duplex Composer

## Breath usage of the program
duplicate composer session or create new session on console environment to work simultaneously without needing to use the same session for everyone.

# **Operations Guide**

## **Transfer Operations**  
These commands allow the transfer of packages, configurations, or entire sessions between environments.  

- `--transfer-packages-from <name>`: Transfers package dependencies from the specified source.  
- `--transfer-configs-from <name>`: Moves configuration settings from a specified source.  
- `--transfer-whole-session <name>`: Transfers an entire session, including configurations and packages.  

## **Create, Destroy & Fix Operations**  
These commands help manage sessions, validate configurations, and update environments.  

- `--new-session <name>`: Creates a new session with the given name.  
- `--clone-session <name>`: Duplicates an existing session.  
- `--destroy <name>`: Deletes a session permanently.  
- `--validate-configuration-of <name>`: Checks and ensures the configuration of the specified session is correct.  
- `--update-packages <name>`: Updates all packages within the specified session.  
- `--environment <name>`: Sets the execution environment for the session.  
- `--execute <command>`: Runs a specified command.  
  - `| --composer`: Executes Composer-related commands.  
  - `| other php extension…`: Executes any additional PHP extensions.


## **Session Management**  
These commands allow the creation of new sessions, setting them as default, and transferring data between sessions.  

- `Duplex --new-session <name> --environment`  
  *Creates a new session and makes it the default environment.*  

- `Duplex --new-session <name> --transfer-whole-session <name>`  
  *Transfers all session data, including configurations and packages, to the new session.*  

- `Duplex --new-session <name> --transfer-packages-from <name>`  
  *Transfers only package dependencies from the specified session to the new session.*  

- `Duplex --new-session <name> --transfer-configs-from <name>`  
  *Transfers only the configuration settings from the specified session to the new session.*  

## **Package Management**  
Commands for installing packages within a session.  

- `Duplex --execute install <package>`  
  *Installs the specified package in the current session.*  


## **Duplex Initialization**  
This command initializes the **Universal Session Package Manager**, enabling duplex communication.  

- `--init <UniversalSessionPackageManager>`: Initializes the universal package manager to manage and synchronize session environments.

# **Package Managers & OS Support**  

## **Programming Language Package Managers**  

| **Programming Language** | **Package/Library Manager**                          | **Supported?** |
|-------------------------|----------------------------------------------------|---------------|
| Python                  | pip, conda, poetry, pipenv                         | ✅🌎         |
| JavaScript/Node.js      | npm, yarn, pnpm                                   | ✅🌎          |
| Ruby                    | RubyGems, Bundler                                 | ❌           |
| Java                    | Maven, Gradle, Apache Ivy                         | ✅           |
| PHP                     | Composer                                         | ✅           |
| C/C++                   | vcpkg, Conan, Hunter                              | ✅           |
| Go                      | go get, Go modules, dep (deprecated)              | ✅           |
| Rust                    | cargo                                            | ✅           |
| Swift                   | CocoaPods, Carthage, Swift Package Manager (SPM) | ✅           |
| .NET (C#)               | NuGet                                            | ✅           |
| R                       | install.packages(), renv                          | ❌           |
| Haskell                 | Cabal, Stack                                      | ❌           |
| Elixir                  | Mix                                              | ❌           |
| Perl                    | CPAN                                             | ❌           |

## **OS Support**  

| **Operating System** | **Does Support It?** | **Remade in Language** |
|----------------------|---------------------|------------------------|
| Windows 10 / 11     | ✅                  | C++                    |
| MacOS X             | ❌                  | Python                 |
| Linux               | ❌                  | Python                 |

