 Making use of one of OpenZeppelin’s smart contracts, we’ll first need to install the OpenZeppelin dependency. 
Forge manages dependencies using git submodules by default, which means that it works with any GitHub repository that contains smart contracts.

Using the forge install command for installing dependencies.

Run the command below in your terminal:

forge install OpenZeppelin/openzeppelin-contracts



Forge will download the OpenZeppelin smart contracts library from GitHub and install it in your project's directory. 

The forge install command has the following syntax:
forge install <dependency>

Where dependency is the name of the dependency that you want to install. In this case, the dependency is OpenZeppelin/openzeppelin-contracts. Once the OpenZeppelin smart contracts library has been installed, you can import the contracts that you need into your project's code.

After installing our dependencies - editing our remappings file. If we try to import an OpenZeppelin smart contract now, we’ll get an error message of “Source file not found”. This can be resolved using a remappings file, which allows us to map a virtual path to a local file system path. By using a remappings file, you can specify the exact location of the required source file, which helps the compiler to resolve the import statements correctly.

To generate this remappings file, run the command below in your terminal:

forge remappings > remappings.txt



Once done, Look for a remappings.txt file created in your project directory, with its content looking similar to the image above.
