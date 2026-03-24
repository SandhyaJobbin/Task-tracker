This is the prompt that can be used:
"Create a Google Apps Script web application that provides a side-by-side comparison interface for two content inputs: Previous Version and Current Version.
UI Requirements
Two large text input fields placed side-by-side:
Left: Previous Version
Right: Current Version
Inputs must support HTML, rich text, or any code format without breaking formatting.
A button labeled 'Analyze Changes' below both fields.
The application must be responsive and work seamlessly across mobile, tablet, and desktop devices.

Core Functionality
When the user clicks 'Analyze Changes', the system should:
1. Perform Content Analysis
Compute:
Total word count (Previous vs Current)
Word count difference
Words added
Words removed
Ignore HTML tags when calculating word counts but preserve them for comparison view.

2. Generate Output Sections**
A. Smart Summary (Top Right Section)
Provide a clear 2-line human-readable summary of:
What changed
Why the change might have been made

B. Key Observations
Automatically detect and list:
Timeline or date updates
Newly added substantial paragraphs
Pricing or currency changes
Structural/content shifts
Any other significant modifications

C. Detailed Difference View
Show a split-screen comparison:
Left: Previous Version
Right: Current Version
Highlight:
Additions (e.g., green)
Deletions (e.g., red)
Modifications (e.g., yellow)
Preserve original formatting (HTML/code-safe rendering)

D. Metadata Extraction (If Available)
Attempt to extract:
Author name
Last modified by
If not found, display "Not available"

E. Scoring & Recommendations
Provide a quality score (0-10) for both versions based on:
Readability
Structure
Clarity
Include:
Improvement suggestions for the current version

Technical Requirements
Use Google Apps Script (HTML Service + Client-side JS)
Ensure fast, near real-time analysis (optimize for performance)
Use efficient diff algorithms (e.g., word-based diff)
Maintain clean, modular, and well-commented code

Output Expectations
Clean, professional UI
Structured output sections (Summary, Observations, Differences, Score)
Accurate and meaningful analysis without unnecessary verbosity

Additional Constraint
The application should not break when large HTML content is pasted.
Ensure security by sanitizing inputs where required."
