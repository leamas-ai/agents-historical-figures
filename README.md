# Historical Figures Debate Agents for Claude Code

This repository contains custom Claude Code sub-agents that allow historical figures to debate contemporary topics while Claude acts as a neutral moderator.

## Quick Installation with leamas

The easiest way to install these agents is using [leamas](https://github.com/leamas-ai/leamas.sh). After leamas has been installed you can run:

```bash
# Install historical figures debate agents for Claude Code
leamas agent@agents-historical-figures
```
From your project directory to install all of the agents and then begin you discussion. Once installed, the agents will be available in your Claude Code environment and can be invoked using the Task tool with their agent names.


## Installation via GitHub

To install from GitHub to your global Claude Code instance:

```bash
cd ~/.claude/agents
git clone https://github.com/leamas-ai/agents-historical-figures.git
```

Or to install only to your project, change into your project directory and run:

```bash
cd .claude/agents
git clone https://github.com/leamas-ai/agents-historical-figures.git
```

If you do not have a `.claude/agents` directory, then create it before running the `git` commands.

## How to Use

### Basic Historical Debate Setup

1. **Start a debate on any contemporary topic**:
   ```
   I want to organize a debate on [topic] between historical figures. 
   Please use:
   - The debate-moderator agent to facilitate
   - [Choose 2-4 historical figure agents] as participants
   ```

2. **Example debate prompt**:
   ```
   Please organize a debate on "The role of artificial intelligence in society" with:
   - debate-moderator as the facilitator
   - socrates-agent, aristotle-agent, and marie-curie-agent as participants
   
   Have them discuss AI ethics, benefits, and risks from their unique perspectives.
   ```

### Advanced Usage

#### 1. **One-on-One Philosophical Dialogue**
   ```
   Have Socrates and Aristotle discuss the nature of knowledge, 
   with the moderator guiding their conversation.
   ```

#### 2. **Historical Advisory Panel**
   ```
   I need advice on [modern issue]. Please convene a panel with 
   Einstein, da Vinci, and Marcus Aurelius to provide their perspectives.
   ```

#### 3. **Cross-Era Scientific Discussion**
   ```
   Have Marie Curie and Albert Einstein debate with Leonardo da Vinci 
   about the relationship between art and science.
   ```

#### 4. **Ethical Dilemma Analysis**
   ```
   Present this ethical dilemma to Socrates, Marcus Aurelius, and Aristotle:
   [describe dilemma]
   Have them explore it from their philosophical frameworks.
   ```

#### 5. **Innovation Workshop**
   ```
   Use Leonardo da Vinci and Einstein agents to brainstorm solutions 
   for [contemporary problem], with the moderator synthesizing ideas.
   ```

## Features and Capabilities

### Debate Structure
The moderator agent follows this format:
1. **Opening** - Topic introduction and participant introductions
2. **Initial Positions** - Each figure states their stance
3. **Rebuttals** - Responses to initial positions
4. **Open Discussion** - Guided free-form debate
5. **Closing Statements** - Final thoughts from each participant
6. **Synthesis** - Moderator's balanced summary

### Agent Characteristics

- **Authentic Voice**: Each agent maintains their historical personality and speaking style
- **Philosophical Consistency**: Arguments align with their known beliefs and methods
- **Modern Adaptation**: Can engage with contemporary concepts while maintaining historical perspective
- **Interactive Depth**: Agents respond to each other's arguments dynamically

### Special Capabilities

1. **Cross-Temporal Understanding**: Historical figures can grasp modern concepts when explained
2. **Philosophical Integration**: Different schools of thought interact meaningfully
3. **Practical Application**: Historical wisdom applied to contemporary challenges
4. **Educational Value**: Learn philosophy and history through engaging dialogue

## Example Commands

### Quick Start
```
"Moderate a debate between Socrates and Einstein on whether truth is absolute or relative"
```

### Complex Scenario
```
"I want to explore the ethics of genetic engineering. Please organize a panel with:
- Aristotle for virtue ethics perspective
- Marcus Aurelius for Stoic view on nature
- Marie Curie for scientific progress angle
- Leonardo da Vinci for innovation and human enhancement
Let them discuss for 5 rounds with the moderator guiding."
```

### Educational Use
```
"Help me understand different philosophical approaches to happiness by having 
Aristotle (eudaimonia), Marcus Aurelius (Stoic contentment), and Socrates 
(examined life) explain their views in a moderated discussion"
```

## Tips for Best Results

1. **Be Specific**: Clearly state the topic and which agents you want to use
2. **Set Context**: Provide background on contemporary issues for historical figures
3. **Guide Direction**: Tell the moderator to focus on specific aspects if needed
4. **Multiple Rounds**: Request multiple rounds of debate for deeper exploration
5. **Ask for Summaries**: Request the moderator to synthesize key insights

## Extending the System

To add new historical figures:
1. Create a new `.md` file in the `agents/` directory
2. Include sections for: Core Identity, Speaking Style, Key Beliefs, Debate Approach
3. Ensure the agent can engage with modern topics while maintaining historical authenticity
4. Test the agent in debates with existing figures

## Notes

- Agents work best when given clear topics and debate structures
- The moderator ensures balanced participation and civil discourse
- Historical figures maintain their authentic worldviews while engaging modern topics
- Debates can be educational, entertaining, and provide unique insights

## Available Agents

### Debate Moderator
- **File**: `agents/debate-moderator.md`
- **Role**: Neutral facilitator of intellectual discourse
- **Features**: Structured debate format, balanced moderation, synthesis of arguments

### Historical Figures

#### Political & Military Leaders

1. **Julius Caesar** (`agents/julius-caesar-agent.md`)
   - Roman general, statesman, and dictator (100-44 BCE)
   - Military genius and political reformer
   - Transformed the Roman Republic into Empire

2. **Alexander the Great** (`agents/alexander-the-great-agent.md`)
   - Macedonian king and military conqueror (356-323 BCE)
   - Created one of history's largest empires by age 30
   - Never lost a battle in 15 years of conquest

3. **Napoleon Bonaparte** (`agents/napoleon-bonaparte-agent.md`)
   - French emperor and military genius (1769-1821)
   - Revolutionized warfare, law, and administration
   - Conquered much of Europe through strategic brilliance

4. **George Washington** (`agents/george-washington-agent.md`)
   - First U.S. President and Revolutionary War general (1732-1799)
   - Father of His Country who established democratic precedents
   - Led ragtag army to defeat British Empire

5. **Winston Churchill** (`agents/winston-churchill-agent.md`)
   - British Prime Minister during WWII (1874-1965)
   - Led Britain through darkest hour with stirring oratory
   - Warning voice against totalitarian threats

6. **Cleopatra VII** (`agents/cleopatra-vii-agent.md`)
   - Last active pharaoh of Egypt (69-30 BCE)
   - Scholar-queen who wielded intelligence and political acumen
   - Preserved Egyptian independence through Roman alliances

7. **Mahatma Gandhi** (`agents/mahatma-gandhi-agent.md`)
   - Leader of Indian independence movement (1869-1948)
   - Pioneer of non-violent resistance and civil disobedience
   - Transformed satyagraha into powerful force for social change

8. **Abraham Lincoln** (`agents/abraham-lincoln-agent.md`)
   - 16th U.S. President during Civil War (1809-1865)
   - Great Emancipator who ended slavery in America
   - Preserved Union through moral leadership

9. **Nelson Mandela** (`agents/nelson-mandela-agent.md`)
   - Anti-apartheid leader and President of South Africa (1918-2013)
   - Spent 27 years in prison, emerged to lead peaceful transition
   - Global symbol of reconciliation and moral leadership

10. **Genghis Khan** (`agents/genghis-khan-agent.md`)
    - Founder of the Mongol Empire (c.1162-1227)
    - Created largest contiguous land empire in history
    - Transformed Eurasian civilization through conquest

#### Scientists & Inventors

11. **Isaac Newton** (`agents/isaac-newton-agent.md`)
    - Mathematical genius who formulated laws of motion and gravity (1642-1727)
    - Invented calculus and revolutionized understanding of light
    - Created mathematical framework for describing nature

12. **Nikola Tesla** (`agents/nikola-tesla-agent.md`)
    - Visionary inventor and electrical engineer (1856-1943)
    - Pioneered alternating current and wireless technology
    - Imagined future of free energy for all humanity

13. **Ada Lovelace** (`agents/ada-lovelace-agent.md`)
    - Considered the first computer programmer (1815-1852)
    - Victorian mathematician who envisioned computing's potential
    - Blended imagination with mathematical precision

14. **Thomas Edison** (`agents/thomas-edison-agent.md`)
    - Prolific American inventor and businessman (1847-1931)
    - Developed light bulb, phonograph, and motion pictures
    - Created first industrial research laboratory

15. **Rosalind Franklin** (`agents/rosalind-franklin-agent.md`)
    - British X-ray crystallographer (1920-1958)
    - Key contributor to DNA structure discovery
    - Precise research initially overlooked but later recognized

16. **Albert Einstein** (`agents/albert-einstein-agent.md`)
    - Theoretical physicist (1879-1955)
    - Revolutionary thinker on space, time, and reality
    - Humanitarian and philosopher-scientist

#### Philosophers & Thinkers

17. **Plato** (`agents/plato-agent.md`)
    - Student of Socrates, writer of philosophical dialogues (428-348 BCE)
    - Founded the Academy and explored ideal forms
    - Established foundations of Western philosophical thought

18. **Laozi** (`agents/laozi-agent.md`)
    - Founder of Taoism (6th century BCE)
    - Ancient Chinese sage who taught the Way of natural harmony
    - Advocated effortless action and wisdom of simplicity

19. **Immanuel Kant** (`agents/immanuel-kant-agent.md`)
    - German Enlightenment philosopher (1724-1804)
    - Established critical philosophy and moral imperatives
    - Defined limits of human reason through systematic analysis

20. **Karl Marx** (`agents/karl-marx-agent.md`)
    - Philosopher and economist who developed Marxism (1818-1883)
    - Analyzed capitalism's contradictions and class struggle
    - Envisioned communist revolution as history's inevitable progression

21. **Friedrich Nietzsche** (`agents/friedrich-nietzsche-agent.md`)
    - German philosopher known for critiques of religion (1844-1900)
    - Proclaimed death of God and envisioned the Übermensch
    - Challenged traditional morality and values

22. **John Locke** (`agents/john-locke-agent.md`)
    - Enlightenment thinker on liberalism (1632-1704)
    - Established liberal political theory and natural rights
    - Founded empirical philosophy and religious tolerance

23. **René Descartes** (`agents/rene-descartes-agent.md`)
    - French philosopher and mathematician (1596-1650)
    - Father of modern philosophy through methodical doubt
    - Established rationalism and founded analytic geometry

24. **Socrates** (`agents/socrates-agent.md`)
    - Classical Greek philosopher (470-399 BCE)
    - Uses Socratic method of questioning
    - Focuses on ethical and definitional inquiries

25. **Aristotle** (`agents/aristotle-agent.md`)
    - Greek philosopher and polymath (384-322 BCE)
    - Systematic, empirical approach
    - Expertise in logic, ethics, politics, and natural science

26. **Marcus Aurelius** (`agents/marcus-aurelius-agent.md`)
    - Roman Emperor and Stoic philosopher (121-180 CE)
    - Practical wisdom from leadership experience
    - Focus on what's within our control

27. **Confucius** (`agents/confucius-agent.md`)
    - Chinese philosopher and teacher (551-479 BCE)
    - Emphasized moral education and social harmony
    - Founded Confucianism influencing East Asian culture

28. **Ibn Khaldun** (`agents/ibn-khaldun-agent.md`)
    - Arab historiographer and social scientist (1332-1406)
    - Pioneer of modern historiography and sociology
    - Analyzed rise and fall of civilizations

#### Cultural Figures & Artists

29. **William Shakespeare** (`agents/william-shakespeare-agent.md`)
    - English playwright and poet (1564-1616)
    - Master of English language and dramatic poetry
    - Created timeless works exploring human nature

30. **Ludwig van Beethoven** (`agents/ludwig-van-beethoven-agent.md`)
    - German composer (1770-1827)
    - Bridged Classical and Romantic periods
    - Created revolutionary symphonies while battling deafness

31. **Wolfgang Amadeus Mozart** (`agents/wolfgang-amadeus-mozart-agent.md`)
    - Austrian composer (1756-1791)
    - Prodigious talent who created perfect classical works
    - Combined mathematical precision with emotional depth

32. **Michelangelo** (`agents/michelangelo-agent.md`)
    - Italian Renaissance sculptor, painter, and architect (1475-1564)
    - Created transcendent art revealing divine beauty
    - Master of David, Sistine Chapel, and St. Peter's Basilica

33. **Pablo Picasso** (`agents/pablo-picasso-agent.md`)
    - Spanish painter and sculptor (1881-1973)
    - Revolutionized visual art through Cubism
    - Most influential artist of the 20th century

34. **Frida Kahlo** (`agents/frida-kahlo-agent.md`)
    - Mexican painter (1907-1954)
    - Transformed personal pain into powerful self-portraits
    - Icon of strength, Mexican identity, and feminist art

35. **Vincent van Gogh** (`agents/vincent-van-gogh-agent.md`)
    - Dutch post-impressionist painter (1853-1890)
    - Emotional intensity and vibrant colors revolutionized art
    - Created masterworks despite mental illness and poverty

36. **Johann Sebastian Bach** (`agents/johann-sebastian-bach-agent.md`)
    - German Baroque composer (1685-1750)
    - Mathematical precision and spiritual depth
    - Created pinnacle of contrapuntal music

37. **Leo Tolstoy** (`agents/leo-tolstoy-agent.md`)
    - Russian novelist (1828-1910)
    - Created epic works exploring meaning of life
    - Advocated nonviolent resistance and spiritual transformation

38. **Jane Austen** (`agents/jane-austen-agent.md`)
    - English novelist (1775-1817)
    - Witty novels of manners exploring women's lives
    - Insightful social observation in Regency England

#### Additional Historical Figures

39. **Leonardo da Vinci** (`agents/leonardo-da-vinci-agent.md`)
    - Renaissance polymath (1452-1519)
    - Integrates art and science
    - Visual thinking and innovation

40. **Marie Curie** (`agents/marie-curie-agent.md`)
    - Pioneering physicist and chemist (1867-1934)
    - First woman Nobel laureate
    - Advocate for women in science

41. **Charles Darwin** (`agents/charles-darwin-agent.md`)
    - English naturalist (1809-1882)
    - Developed theory of evolution by natural selection
    - Revolutionary understanding of life's diversity

42. **Galileo Galilei** (`agents/galileo-galilei-agent.md`)
    - Italian astronomer and physicist (1564-1642)
    - Father of modern science and scientific method
    - Defended heliocentrism against religious opposition

43. **Harriet Tubman** (`agents/harriet-tubman-agent.md`)
    - American abolitionist and conductor (c.1822-1913)
    - Led Underground Railroad helping slaves escape
    - Civil War spy and women's suffrage activist

44. **Mary Wollstonecraft** (`agents/mary-wollstonecraft-agent.md`)
    - English writer and women's rights advocate (1759-1797)
    - Author of "A Vindication of the Rights of Woman"
    - Pioneer of feminist philosophy and gender equality