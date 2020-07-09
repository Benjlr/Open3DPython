# Open3DPython
Python registration tools for prototyping


To Setup:
1. Pull Git Repo
2. Install Python 3.6
3. In Models.AutomatedRegistration.PythonRegistrationUtils add a new case to the SWITCH statement on line 57. The statement should include:
  - Your PC name
  - The location of the python 3.6 exe on your computer
  - The location of the 'scripts' folder from this repo
  - The location of 'main.py' from this repo.
  
 Below is an example: 

               case "DESKTOP-2J6H0DH":
                    var python36Loc = @"C:\Users\rober\source\repos\Open3DFixed\venv\Scripts\python.exe";
                    myBat.AppendLine($"@cd C:\\Users\\rober\\source\\repos\\Open3DFixed\\venv\\Scripts");
                    myBat.AppendLine($"{python36Loc} C:\\Users\\rober\\source\\repos\\Open3DFixed\\main.py {args[0]} {args[1]} {stageCommand}");

                    break;
