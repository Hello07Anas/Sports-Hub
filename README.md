# The Sports-Hub

// Here small video for the app 

https://github.com/Hello07Anas/Sports-Hub/assets/120333186/fd752176-1650-4b95-b7f8-18afb2e6795d

## Overview
The Sports App is an iOS application designed to provide users with information about various sports, leagues, and teams. It allows users to browse sports, view league details, see upcoming events, check latest results, and manage their favorite leagues.

## Features
- Browse a collection of sports.
- View leagues associated with each sport.
- Mark leagues as favorites and manage them.
- View details of leagues, including upcoming events, latest results, and teams.
- View detailed information about each team.
- Offline support for favorite leagues.
- Elegant and consistent UI across all screens.
- Designed using MVVM design patterns.
- Unit testing with at least 92% code coverage.
- Dependencies: Alamofire, Kingfisher.

## Setup Instructions
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/sports-app.git
    ```
2. Navigate to the project directory:
    ```bash
    cd sports-app
    ```
3. Install dependencies using CocoaPods:
    ```bash
    pod install
    ```
4. Open the project in Xcode:
    ```bash
    open SportsApp.xcworkspace
    ```
5. Build and run the project on your simulator or device.

## Screens

### Main Screen
The main screen contains two tabs:
1. **Sports Tab**:
   - Displays all the sports available in the sports database.
   - Sports are displayed in a `CollectionView` with 2 sports per row.
   - Each item shows the sport's thumbnail (`strSportThumb`) and name (`strSport`).
   - Title: **Sports**.
   - Selecting a sport navigates to the **Leagues ViewController**.

2. **Favorite Leagues Tab**:
   - Displays the user's favorite leagues.
   - Uses CoreData for data persistence.
   - Similar UI to the Leagues ViewController.
   - Online: Clicking a row navigates to the **LeagueDetailsViewController**.
   - Offline: Displays an alert indicating no internet connection.

### Leagues ViewController
- Type: `TableViewController`
- Title: **Leagues**
- Custom rows containing:
  1. Circular league badge (`strBadge`).
  2. League name (`strLeague`).
  3. Button to view league video (`strYoutube`).
- Clicking a row navigates to the **LeagueDetailsViewController**.

### LeagueDetails ViewController
- Divided into three parts with orthogonal scrolling:
  1. **Upcoming Events**: 
     - Horizontal scrolling.
     - Each item shows the event name (`strEvent`), date, and time.
  2. **Latest Results**: 
     - Vertical scrolling.
     - Each item shows the home team, away team, scores, date, and time.
  3. **Teams**: 
     - Horizontal scrolling.
     - Each item shows a circular image of the team.
     - Clicking an image navigates to the **TeamDetails ViewController**.
- Top right corner: Button to add the league to favorite leagues.

### TeamDetails ViewController
- Displays detailed information about the team.
- The UI is designed to be elegant and informative.

## Design Patterns
The app is designed using MVVM to ensure a clean and maintainable codebase.

## Unit Testing
- Network file unit tests with at least 92% code coverage.

## Dependencies
- **Alamofire**: For network requests.
- **Kingfisher**: For image downloading and caching.

## Project Management
- with my Teammate.
- The deadline to deliver  (8 days period).

## Contributors
- Anas Salah: [GitHub Profile](https://github.com/Hello07Anas)
- Ywsoliman: [GitHub Profile](https://github.com/ywsoliman)



