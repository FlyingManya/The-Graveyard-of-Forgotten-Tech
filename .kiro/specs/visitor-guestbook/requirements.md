# Requirements Document

## Introduction

The Visitor Guestbook is a spooky-themed interactive feature that allows visitors to the Graveyard of Forgotten Tech to leave messages, sign their names, and view messages from other visitors. The guestbook maintains the eerie atmosphere while providing a social element to the experience.

## Glossary

- **Visitor**: A user who accesses the Graveyard of Forgotten Tech website
- **Entry**: A single message/signature left by a visitor in the guestbook
- **Guestbook System**: The complete system for creating, storing, and displaying visitor entries
- **LocalStorage**: Browser-based storage mechanism for persisting guestbook entries
- **Timestamp**: The date and time when an entry was created

## Requirements

### Requirement 1

**User Story:** As a visitor, I want to leave a message in the guestbook, so that I can share my thoughts about the experience with others.

#### Acceptance Criteria

1. WHEN a visitor enters their name and message THEN the Guestbook System SHALL validate that both fields are non-empty
2. WHEN a visitor submits a valid entry THEN the Guestbook System SHALL store the entry with name, message, and timestamp
3. WHEN an entry is successfully submitted THEN the Guestbook System SHALL clear the input fields and display a confirmation
4. WHEN a visitor attempts to submit with empty fields THEN the Guestbook System SHALL prevent submission and display an error message
5. WHEN an entry is created THEN the Guestbook System SHALL automatically add the current timestamp

### Requirement 2

**User Story:** As a visitor, I want to view all guestbook entries, so that I can read what others have written about their experience.

#### Acceptance Criteria

1. WHEN the guestbook page loads THEN the Guestbook System SHALL display all stored entries in reverse chronological order
2. WHEN displaying entries THEN the Guestbook System SHALL show the visitor name, message, and formatted timestamp for each entry
3. WHEN there are no entries THEN the Guestbook System SHALL display a welcoming message encouraging the first entry
4. WHEN entries exceed the visible area THEN the Guestbook System SHALL provide scrolling functionality
5. WHEN a new entry is added THEN the Guestbook System SHALL update the display immediately without page reload

### Requirement 3

**User Story:** As a visitor, I want the guestbook to have a spooky theme, so that it matches the overall aesthetic of the website.

#### Acceptance Criteria

1. WHEN the guestbook is displayed THEN the Guestbook System SHALL use the purple and dark color scheme consistent with the site
2. WHEN displaying entries THEN the Guestbook System SHALL style them as vintage paper or tombstone cards
3. WHEN animations occur THEN the Guestbook System SHALL use subtle spooky effects like fading or glowing
4. WHEN the page loads THEN the Guestbook System SHALL include ghost emoji 👻 in the title
5. WHEN interactive elements are hovered THEN the Guestbook System SHALL provide visual feedback with purple glow effects

### Requirement 4

**User Story:** As a visitor, I want my guestbook entries to persist, so that they remain visible even after I close the browser.

#### Acceptance Criteria

1. WHEN an entry is submitted THEN the Guestbook System SHALL save it to browser localStorage immediately
2. WHEN the page is reloaded THEN the Guestbook System SHALL retrieve and display all previously saved entries
3. WHEN localStorage is unavailable THEN the Guestbook System SHALL display a warning message to the visitor
4. WHEN entries are stored THEN the Guestbook System SHALL use JSON format for data serialization
5. WHEN the storage limit is reached THEN the Guestbook System SHALL notify the visitor and prevent new entries

### Requirement 5

**User Story:** As a visitor, I want to see how long ago entries were posted, so that I can understand the timeline of visitor activity.

#### Acceptance Criteria

1. WHEN displaying timestamps THEN the Guestbook System SHALL format them as relative time (e.g., "2 hours ago", "3 days ago")
2. WHEN an entry is less than 1 minute old THEN the Guestbook System SHALL display "Just now"
3. WHEN an entry is less than 1 hour old THEN the Guestbook System SHALL display minutes (e.g., "15 minutes ago")
4. WHEN an entry is less than 24 hours old THEN the Guestbook System SHALL display hours (e.g., "5 hours ago")
5. WHEN an entry is older than 24 hours THEN the Guestbook System SHALL display days (e.g., "3 days ago")

### Requirement 6

**User Story:** As a visitor, I want to access the guestbook from the main menu, so that I can easily find and use this feature.

#### Acceptance Criteria

1. WHEN the main menu is displayed THEN the Guestbook System SHALL provide a clearly visible button to access the guestbook
2. WHEN the guestbook button is clicked THEN the Guestbook System SHALL navigate to the guestbook page
3. WHEN on the guestbook page THEN the Guestbook System SHALL provide a back button to return to the main menu
4. WHEN navigation occurs THEN the Guestbook System SHALL maintain consistent styling with other pages
5. WHEN the guestbook button is hovered THEN the Guestbook System SHALL display a tooltip or visual effect

### Requirement 7

**User Story:** As a visitor, I want input validation and sanitization, so that the guestbook remains safe and appropriate.

#### Acceptance Criteria

1. WHEN a visitor enters a name THEN the Guestbook System SHALL limit it to 50 characters maximum
2. WHEN a visitor enters a message THEN the Guestbook System SHALL limit it to 500 characters maximum
3. WHEN displaying entries THEN the Guestbook System SHALL escape HTML to prevent script injection
4. WHEN validating input THEN the Guestbook System SHALL trim whitespace from both ends
5. WHEN a character limit is reached THEN the Guestbook System SHALL display the remaining character count
