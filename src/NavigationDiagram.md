```mermaid
flowchart TD

    Login --> UserName --> Email+Number --> Password --> Verify --> |sign up| Login
    Login --> |log in| Landing

    Landing --> |create| ClubName
    Landing --> Settings
    Landing --> SearchClub
    Landing --> |member| ClubMember
    Landing --> |owner| ClubOwner
    
    ClubName --> ClubAbout --> SendInvites
    
    Settings --> |sign out| Login

    SearchClub --> ClubPreview --> |join| ClubMember

    ClubOwner --> |additional invites| SendInvites
    SendInvites --> |done| ClubOwner
```
