# World of Warcraft: Midnight - Testing Tracker

## Overview
This document tracks testing progress for addon features and game features in preparation for the World of Warcraft expansion **Midnight**.

---

## Addon Testing

### Core Addon Functionality
- [ ] **UI Framework Updates**
  - [ ] Interface compatibility with new UI elements
  - [ ] Frame positioning and scaling
  - [ ] Event handling for new game events
  
- [ ] **API Changes**
  - [ ] Deprecated function replacements
  - [ ] New API endpoints integration
  - [ ] Secure function call updates

- [ ] **Performance Testing**
  - [ ] Memory usage optimization
  - [ ] FPS impact assessment
  - [ ] Loading time improvements

### Specific Addon Categories

#### **Combat Addons**
- [ ] Damage meters
- [ ] Threat meters
- [ ] Combat logging
- [ ] Rotation helpers

#### **UI Enhancement Addons**
- [ ] Action bar modifications
- [ ] Unit frame customization
- [ ] Minimap enhancements
- [ ] Bag organization

#### **Utility Addons**
- [ ] Quest helpers
- [ ] Auction house tools
- [ ] Guild management
- [ ] Character statistics

#### **Font and Media Systems**
- [ ] **LibSharedMedia Integration**
  - _For all LibSharedMedia integration tests, we will use the NoobTacoUI-Media (NTUI-media) addon as the primary test media source. This ensures consistent, real-world testing of custom fonts, audio, and graphics. See [NTUI-media LSM Integration Test Case](test-cases/ntui-media-lsm-integration.md) for detailed steps._
  - [ ] Font replacement functionality
  - ✅ External fonts directory compatibility
  - [ ] Custom font loading and validation
  - [ ] Font fallback mechanisms
  - ✅ [External fonts directory compatibility](test-cases/external-fonts-directory-compatibility.md) _(Pass: system and in-game font replacement confirmed)_
- [ ] **External Fonts Directory Testing**
  - [ ] Font file detection in external directories
  - [ ] Font registration with LibSharedMedia
  - [ ] Cross-addon font sharing
  - [ ] Font caching and performance impact
- [ ] **External Icons Directory Testing**
  - [ ] [External ICONS directory compatibility (TC-002)](test-cases/external-icons-directory-compatibility.md)
  - [ ] Icon file detection and registration
  - [ ] Cross-addon icon sharing
  - [ ] Icon caching and performance impact

#### **Housing System Addons**
- [ ] **Housing Management Addons**
  - [ ] House navigation and teleportation
  - [ ] Décor inventory management
  - [ ] Housing achievement tracking
  - [ ] Neighborhood directory and social features
- [ ] **Decoration and Design Addons**
  - [ ] Advanced placement tools
  - [ ] Decoration cataloging and search
  - [ ] Room planning and layout tools
  - [ ] Color coordination and theming assistants
- [ ] **Guild Housing Integration**
  - [ ] Guild house permission management
  - [ ] Guild decoration contribution tracking
  - [ ] Guild neighborhood coordination tools
  - [ ] Guild housing event scheduling
- [ ] **Housing API Integration**
  - [ ] New housing-related game events
  - [ ] Housing state detection and monitoring
  - [ ] Decoration placement API calls
  - [ ] Neighborhood and Endeavor status tracking

#### **PvP Addons**
- [ ] Battleground timers
- [ ] Arena frames
- [ ] PvP statistics
- [ ] Enemy cooldown tracking

---

## Game Features Testing

### New Midnight Features
- [ ] **Housing System** *(Major New Feature)*
  - [ ] **House Acquisition and Management**
    - [ ] Initial house claiming process
    - [ ] Warband house sharing functionality
    - [ ] Cross-faction house access (Orc in Alliance house, etc.)
    - [ ] Multiple character access validation
    
  - [ ] **Neighborhood Systems**
    - [ ] **Alliance Neighborhood - Founder's Point**
      - [ ] Zone exploration and mapping
      - [ ] Plot selection and variety testing
      - [ ] Biome diversity (spooky forests, autumnal farmland)
      - [ ] Central hub functionality and NPC activity
    - [ ] **Horde Neighborhood - Razorwind Shores**
      - [ ] Zone exploration and mapping  
      - [ ] Plot selection and variety testing
      - [ ] Biome diversity (lush oases, windswept bluffs)
      - [ ] Central hub functionality and NPC activity
    - [ ] **Plot Types and Locations**
      - [ ] Hermit plots (isolated locations)
      - [ ] Small cul-de-sacs (2-3 houses for friends)
      - [ ] Large groupings (bustling areas)
      - [ ] Plot size consistency (~50 plots per neighborhood)
      
  - [ ] **Neighborhood Types**
    - [ ] **Public Neighborhoods**
      - [ ] Auto-creation as servers fill up
      - [ ] Semi-procedural naming system
      - [ ] Server-managed organization
      - [ ] Availability and scaling testing
    - [ ] **Private Neighborhoods**
      - [ ] **Guild Neighborhoods**
        - [ ] Guild creation and management
        - [ ] Guild member permissions
        - [ ] Guild house coordination
      - [ ] **Charter Neighborhoods**
        - [ ] Player group creation
        - [ ] Charter management systems
        - [ ] Group coordination tools
        
  - [ ] **Customization Systems**
    - [ ] **Interior Design**
      - [ ] Basic Mode functionality
      - [ ] Advanced Mode capabilities
      - [ ] Décor placement and positioning
      - [ ] Item resizing functionality
      - [ ] Dye system for select items
      - [ ] Free placement validation (anywhere in house)
    - [ ] **Exterior Customization**
      - [ ] Barber shop-like interface
      - [ ] **Themed Kits Testing**
        - [ ] Blood Elf theming
        - [ ] Night Elf theming
        - [ ] Orc theming
        - [ ] Human theming
      - [ ] **Architecture Components**
        - [ ] Tower variations
        - [ ] Window options
        - [ ] Facade selections
        - [ ] Cross-faction restrictions (Alliance/Horde neighborhoods)
        - [ ] Neutral architecture in both neighborhoods
        
  - [ ] **Endeavors System**
    - [ ] Monthly Endeavor activation (~once per month)
    - [ ] **Public Neighborhood Endeavors**
      - [ ] Server-selected Endeavor testing
      - [ ] Task completion mechanics
      - [ ] NPC spawning and decoration unlocks
    - [ ] **Private Neighborhood Endeavors**
      - [ ] Player selection from Endeavor options
      - [ ] Special world event Endeavors
    - [ ] **Scaling and Requirements**
      - [ ] Task scaling by neighborhood size
      - [ ] Activity-based requirement adjustments
      - [ ] Visual decoration changes during Endeavors
    - [ ] **Specific Endeavor Testing**
      - [ ] Mechagon Endeavor (from screenshots)
      - [ ] Pandaria-themed Endeavors
      - [ ] Various faction/culture Endeavors
      
  - [ ] **Reward and Collection Systems**
    - [ ] **Décor Acquisition Methods**
      - [ ] Achievement rewards (e.g., Onyxia defeat)
      - [ ] Profession crafting
      - [ ] Quest rewards (e.g., jade-inlaid bookshelf from Pandaria)
      - [ ] Vendor purchases
      - [ ] Auction House trading
      - [ ] General adventuring drops
    - [ ] **Warband Sharing**
      - [ ] Cross-character décor collection access
      - [ ] Reward persistence across characters
      - [ ] Collection synchronization
      
  - [ ] **Performance and Technical**
    - [ ] Housing zone loading times
    - [ ] Neighborhood instancing performance
    - [ ] Decoration rendering optimization
    - [ ] Cross-faction functionality stability
    - [ ] Large decoration collections impact

- [ ] **New Zones**
  - [ ] Zone exploration and mapping
  - [ ] Quest chains and storylines
  - [ ] Environmental interactions
  - [ ] Performance in new areas

- [ ] **Character Progression**
  - [ ] New talent systems
  - [ ] Skill point allocation
  - [ ] Character customization options
  - [ ] Level cap changes

- [ ] **Combat Systems**
  - [ ] New abilities and spells
  - [ ] Combat mechanics changes
  - [ ] Class balance adjustments
  - [ ] PvP system updates

- [ ] **Social Features**
  - [ ] Guild system improvements
  - [ ] Cross-realm functionality
  - [ ] Communication tools
  - [ ] Group finder enhancements

### Existing Feature Compatibility
- [ ] **Legacy Content**
  - [ ] Old zone accessibility
  - [ ] Previous expansion content
  - [ ] Achievement system
  - [ ] Mount and pet collections

- [ ] **Core Systems**
  - [ ] Trading and economy
  - [ ] Crafting professions
  - [ ] Mail system
  - [ ] Calendar functionality

---

## Testing Methodology

### Test Environments
- [ ] **PTR (Public Test Realm)**
  - Environment: `PTR Server`
  - Client Version: `[Version Number]`
  - Testing Period: `[Date Range]`

- [ ] **Beta Testing**
  - Environment: `Beta Client`
  - Client Version: `[Version Number]`
  - Testing Period: `[Date Range]`

- [ ] **Live Server Preparation**
  - Environment: `Live Realm`
  - Backup Strategy: `[Backup Plan]`
  - Rollback Plan: `[Contingency Plan]`

### Test Cases Template
```markdown
#### Test Case: [Feature Name]
- **Objective:** [What are we testing?]
- **Prerequisites:** [What needs to be set up?]
- **Steps:**
  1. [Step 1]
  2. [Step 2]
  3. [Step 3]
- **Expected Result:** [What should happen?]
- **Actual Result:** [What actually happened?]
- **Status:** [ ] Pass / [ ] Fail / [ ] Blocked
- **Notes:** [Additional observations]
- **Date Tested:** [Date]
- **Tester:** [Name/Handle]
```

---

## Issues and Bug Reports

### Critical Issues
| Issue ID | Description | Severity | Status | Assignee | Date Reported |
|----------|-------------|----------|---------|----------|---------------|
|          |             |          |         |          |               |

### Known Limitations
| Feature | Limitation | Workaround | Timeline |
|---------|------------|------------|----------|
|         |            |            |          |

---

## Housing Documentation and Screenshots

### Screenshot Collection Checklist
- [ ] **Neighborhood Overview Shots**
  - [ ] Founder's Point (Alliance) - full neighborhood view
  - [ ] Razorwind Shores (Horde) - full neighborhood view
  - [ ] Different biomes within each neighborhood
  - [ ] Central hub areas with NPC activity
  
- [ ] **House Exterior Variations**
  - [ ] Blood Elf themed exteriors
  - [ ] Night Elf themed exteriors  
  - [ ] Orc themed exteriors
  - [ ] Human themed exteriors
  - [ ] Different tower, window, and facade combinations
  
- [ ] **Interior Customization Examples**
  - [ ] Basic Mode decoration interface
  - [ ] Advanced Mode decoration interface
  - [ ] Various room layouts and designs
  - [ ] Décor placement and resizing examples
  - [ ] Dye system demonstrations
  
- [ ] **Endeavor Visual Changes**
  - [ ] Before/after Endeavor activation
  - [ ] Mechagon Endeavor decorations
  - [ ] Various cultural theme Endeavors
  - [ ] NPC additions during Endeavors
  
- [ ] **Guild and Social Features**
  - [ ] Guild neighborhood management interfaces
  - [ ] Charter neighborhood creation
  - [ ] Cross-faction house visits
  - [ ] Warband house sharing demonstrations

### Information Gathering Priorities
- [ ] **Housing API Documentation**
  - [ ] New function calls and events
  - [ ] Housing state variables
  - [ ] Decoration manipulation methods
  - [ ] Neighborhood and Endeavor APIs
  
- [ ] **Guild Control Systems**
  - [ ] Guild housing permissions structure
  - [ ] Guild neighborhood creation process
  - [ ] Guild member access levels
  - [ ] Guild decoration sharing policies
  
- [ ] **Technical Specifications**
  - [ ] Housing zone technical limits
  - [ ] Decoration count maximums
  - [ ] Performance optimization requirements
  - [ ] Cross-realm functionality details

### Reference Links for Housing
- [Housing 3D Tour](https://worldofwarcraft.blizzard.com/en-us/housing)
- [Building in Azeroth: A First Look at Housing](https://worldofwarcraft.blizzard.com/news/24176592)
- [Azeroth Beautiful: Housing Interior Design](https://worldofwarcraft.blizzard.com/news/24186690/)
- [Azeroth Living: Housing Rewards](https://worldofwarcraft.blizzard.com/news/24196547/)
- [WoW Housing: It's Only Neighborly](https://worldofwarcraft.blizzard.com/news/24221516/)
- [Housing Announcement](https://worldofwarcraft.blizzard.com/en-us/news/24230692)

---

## Resources and References

### Official Documentation
- [WoW API Documentation](https://wowpedia.fandom.com/wiki/World_of_Warcraft_API)
- [Interface Customization](https://wowpedia.fandom.com/wiki/Interface_customization)
- [Midnight Expansion Notes](https://worldofwarcraft.com/en-us/news)

### Community Resources
- [WowInterface](https://www.wowinterface.com/)
- [CurseForge](https://www.curseforge.com/wow/addons)
- [GitHub WoW Addons](https://github.com/topics/world-of-warcraft-addon)

### Testing Tools
- [ ] **Debugging Addons**
  - BugSack
  - !BugGrabber
  - DevTool
  
- [ ] **Performance Monitoring**
  - CPU Usage addon
  - Memory usage tracking
  - FPS monitoring tools

---

## Timeline and Milestones

### Pre-Launch Testing
- [ ] **Phase 1:** Core addon compatibility (Target: [Date])
- [ ] **Phase 2:** New feature integration (Target: [Date])
- [ ] **Phase 3:** Performance optimization (Target: [Date])
- [ ] **Phase 4:** Final validation (Target: [Date])

### Launch Preparation
- [ ] **Backup creation:** [Date]
- [ ] **Addon updates:** [Date]
- [ ] **Final testing:** [Date]
- [ ] **Go-live readiness:** [Date]

---

## Notes and Observations

### General Notes
- Document any unexpected behaviors or interesting findings here
- Track performance comparisons between current and Midnight versions
- Note any breaking changes that affect multiple addons

### Testing Log
| Date | Activity | Findings | Next Steps |
|------|----------|----------|------------|
|      |          |          |            |

---

*Last Updated: [Date]*  
*Testing Team: [Names/Handles]*  
*Document Version: 1.0*