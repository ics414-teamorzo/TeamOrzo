Required functionality. You are developing a stand-alone application to create .ics event files. You must demonstrate the following are implemented:

### Version (section 3.7.4 of RFC 5545)
• Property Name:  VERSION
• Purpose:  This property specifies the identifier corresponding to the
      highest version number or the minimum and maximum range of the
      iCalendar specification that is required in order to interpret the
      iCalendar object.
• Conformance:  This property MUST be specified once in an iCalendar object.
• Description:  A value of "2.0" corresponds to this memo.
• VERSION:2.0

### Classification (3.8.1.3). Note this is a way of users designating events as public (default), private, or confidential.
• Property Name:  CLASS
• Purpose:  This property defines the access classification for a calendar component.
• CLASS:PUBLIC
    • Not be opaque, but rather transparent, to searches for busy time
• CLASS:PRIVATE 
    • opaque to searches for busy time
• CLASS:CONFIDENTIAL
•  CLASS:TOP-SECRET

### Geographic Position (3.8.1.6)
• Property Name:  GEO
• Purpose:  This property specifies information related to the global position for the activity specified by a calendar component.
•  Value Type:  FLOAT.  The value MUST be two SEMICOLON-separated FLOAT values.
• geovalue   = float ";" float 
             = Latitude and Longitude components
• GEO:37.386013;-122.082932

### Priority (3.8.1.9)
• Property Name:  PRIORITY
•  Purpose:  This property defines the relative priority for a calendar component.
• Description:  This priority is specified as an integer in the range 0
      to 9.  A value of 0 specifies an undefined priority.  A value of 1
      is the highest priority.  A value of 2 is the second highest
      priority.  Subsequent numbers specify a decreasing ordinal
      priority.  A value of 9 is the lowest priority.

• PRIORITY:1
• PRIORITY:2
• PRIORITY:0

### Summary (3.8.1.12)
• Property Name:  SUMMARY
•  Purpose:  This property defines a short summary or subject for the calendar component.
• This property is used in the "VALARM" calendar component to capture the subject of an EMAIL category of alarm.
• SUMMARY:Department Party

### DTSTART (3.8.2.4)
• Property Name:  DTSTART
• Purpose:  This property specifies when the calendar component begins.
• Date-Time Start
• This property is
      REQUIRED in all types of recurring calendar components that
      specify the "RRULE" property.  This property is also REQUIRED in
      "VEVENT" calendar components contained in iCalendar objects that
      don't specify the "METHOD" property.
• DTSTART:19980118T073000Z
• DTSTART:20190728T160000

### DTEND (3.8.2.2)
• Property Name:  DTEND
• Date-Time End
• Purpose:  This property specifies the date and time that a calendar component ends.
• Value MUST match value type
•  DTEND:19960401T150000Z
• DTEND;VALUE=DATE:19980704



### Time zone identifier (3.8.3.1)
• Property Name:  TZID
•  Purpose:  This property specifies the text value that uniquely
      identifies the "VTIMEZONE" calendar component in the scope of an
      iCalendar object.
• value type is either DATE-TIME or TIME and not intended to specify a UTC
      or a "floating" time.  The presence of the SOLIDUS character as a
      prefix, indicates that this "TZID" represents an unique ID in a
      globally defined time zone registry (when such registry is
      defined).
• public-domain TZ database [TZDB](https://tools.ietf.org/html/rfc5545#ref-TZDB)
• Example:  The following are examples of non-globally unique time zone identifiers:

       TZID:America/New_York

       TZID:America/Los_Angeles

• The following is an example of a fictitious globally unique time
      zone identifier:

       TZID:/example.org/America/New_York


Required functionality. You are developing a stand-alone application to create .ics event files. You must demonstrate the following are implemented:
• 
• 
• 
• 
• 
• 

