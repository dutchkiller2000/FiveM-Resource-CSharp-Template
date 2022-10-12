# FiveM Resource CSharp template
No need to create your own c# dev environment and resource.

This C# environment provides you with a setup solution that builds the DLL to the resource folder, and also have a source folder where you can develop your c# resource.
This resource also contains a shared environment. This project will be shared between the server and the client. And it makes it possible to use shared classes like Vector3 from citizenfx.



# Setup

Pull this resource.
Update the nuget packages (Ore make your server artifact the same as the current version)
And start coding :) Dont forget the build the project after you made any changes (Crtl+Shift+B) And restart your resource.

# Updating the nuget package
Open the nuget package: In vs22 go to Tools > NuGet Package Manager> Manage NuGet packages for solution. Update the citizenFx.Core.Client and Server packages here.
Make sure that you dont install the client on the server by accident.

After that go to your solution explorer > Open refrences > Right click on CitizenFX.Core.(Client/Server) > Properties > And set copy to local to false.
This prevent the resource from starting.

Any issues or questions? Feel free to open an issue.