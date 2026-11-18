Class: Book

Attributes:
- title: String
- author: String
- pages: int
- genre: String
- ISBN: String
- rating: double
- readingStatus: String

Relationships:
- N/A

Responsibilities:
- Store information about books
- Allow users to change any information necessary
- Organize books in an ArrayList as they are added

Class: Journal

Attributes:
- title: String
- type: String

Relationships:
- N/A

Responsibilities:
- ability to update title and type
- HTML should handle text?

Class: Story

Attributes:
- title: String
- shortDescription: String
- ArrayList<StoryCharacter>: ArrayList

Relationships:
- Has Chapters and Characters

Responsibilities:
- ability to add/edit/delete characters
- ability to add/edit/delete chapters
- ability to modify title and description

Class: Chapter

Attributes:
- title: String
- type: String

Relationships:
- Is used in the Story class

Responsibilities:
- ability to edit attributes

Class: StoryCharacter

Attributes:
- name: String
- type: String
- age: int
- hairColor: String
- height: double
- mainCharacter: Boolean

Relationships:
- Is used in the Story class

Responsibilities:
- ability to edit attributes

Class: Main

Attributes:
- N/A

Relationships:
-Utilizes all prior mentioned classes directly and/or indirectly

Responsibilities:
- Asks user for input regarding Stories, Books, Journals, Chapters, and StoryCharacters
- Updates information in the appropriate class(s)
- Tests if classes work as they should
- Handles bad input
