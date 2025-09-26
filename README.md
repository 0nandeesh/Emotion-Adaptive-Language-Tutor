# Emotion-Adaptive Language Tutor

An AI-powered multilingual conversation practice application that adapts to your emotional state to provide personalized language learning experiences through realistic, scenario-based conversations.

## Features

- **Emotion-Aware Learning**: Adapts conversation complexity based on your current mood (Confused, Curious, Confident)
- **Multilingual Support**: Practice conversations in English, French, Spanish, German, Kannada, and Japanese
- **Scenario-Based Learning**: Create custom conversation scenarios (airport, restaurant, shopping, etc.)
- **Grammar Analysis**: Get detailed explanations of grammar patterns, idioms, and cultural expressions
- **Named Entity Recognition**: Practice using people, places, and entities from conversations
- **Cultural Context**: Learn politeness cues and cultural behaviors specific to target languages
- **Performance Metrics**: Track response time, token usage, and learning progress
- **Multilingual Interface**: Use the app in English, Kannada, Hindi, or Spanish

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Groq API key (get one from [Groq Console](https://console.groq.com/))

### Installation

1. Clone the repository:
```bash
git clone https://github.com/your-username/emotion-adaptive-language-tutor.git
cd emotion-adaptive-language-tutor
```

2. Install required dependencies:
```bash
pip install streamlit groq python-dotenv pandas matplotlib
```

3. Create a `.env` file in the project root and add your Groq API key:
```env
GROQ_API_KEY=your_groq_api_key_here
```

### Running the Application

Start the Streamlit app:
```bash
streamlit run multilingual_convo_app_env.py
```

The app will open in your default web browser at `http://localhost:8501`

## How to Use

### 1. Configure Your Learning Session
- **Scenario**: Enter a real-world situation (e.g., "At the airport", "Ordering food")
- **Language**: Choose your target language from 6 supported options
- **Roles**: Define your role and the other participant's role
- **Turns**: Set the number of conversation exchanges (4-12)
- **Mood**: Select how you're feeling today to get appropriately adapted content

### 2. Generate Learning Content
Click "Generate Conversation and Grammar Help" to create:
- **Interactive Conversation**: Realistic dialogue with avatar representations
- **Grammar Analysis**: Detailed breakdown of language patterns and structures
- **Cultural Notes**: Politeness cues and cultural context
- **Named Entity Practice**: Exercises using people and places from the conversation

### 3. Track Your Progress
Monitor your learning metrics including response times, token usage, and performance trends over time.

## Emotion-Based Adaptation

The app adapts conversation complexity based on your emotional state:

- **Confused**: Simple language, key word repetition, encouraging tone
- **Curious**: Standard learner-level expressions with moderate variety  
- **Confident**: Advanced idioms, native expressions, challenging content

## Supported Languages

### Conversation Languages
- English
- French
- Spanish
- German
- Kannada
- Japanese

### Interface Languages
- English
- Kannada
- Hindi
- Spanish

## Learning Components

### Grammar Focus
- Tense patterns and usage
- Sentence structure analysis
- Polite forms and formality levels
- At least 3 examples from each conversation

### Cultural Learning
- Politeness expressions
- Regional customs and behaviors
- Appropriate social interactions
- Context-specific vocabulary

### Common Pitfalls
- Typical learner mistakes
- How to avoid errors
- Native speaker alternatives
- Cultural misunderstandings

## Technical Details

### Dependencies
- **Streamlit**: Web application framework
- **Groq**: LLaMA-4 Scout model for AI conversations
- **Pandas**: Data manipulation and analysis
- **Matplotlib**: Performance visualization
- **python-dotenv**: Environment variable management

### AI Model
- Uses Meta's LLaMA-4 Scout 17B model via Groq
- Optimized for multilingual conversation generation
- Cultural context awareness
- Grammar pattern recognition

## Configuration Options

Customize the application by modifying these parameters:

```python
# Conversation settings
TURNS_MIN = 4
TURNS_MAX = 12
TEMPERATURE = 0.8
MAX_TOKENS = 1024

# Supported languages
LANGUAGES = ["English", "French", "Spanish", "German", "Kannada", "Japanese"]
UI_LANGUAGES = ["English", "Kannada", "Hindi", "Spanish"]
```

## Performance Metrics

Track your learning progress with built-in analytics:
- **Response Time**: API call latency
- **Token Usage**: Conversation complexity measure
- **Accuracy Estimation**: Learning effectiveness
- **Progress Visualization**: Historical performance trends

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines
- Follow PEP 8 style guidelines
- Add docstrings for new functions
- Include type hints where possible
- Test multilingual functionality
- Update README for new features

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **Groq** for providing fast LLaMA-4 model access
- **Streamlit** for the intuitive web framework
- **Meta** for the LLaMA language models
- **Flaticon** for avatar icons

## Known Issues

- Avatar images require internet connection
- Some languages may have limited cultural context
- Performance metrics are estimates

## Future Enhancements

- [ ] Voice input/output support
- [ ] More languages (Arabic, Mandarin, Russian)
- [ ] Advanced grammar exercises
- [ ] Progress tracking with user accounts
- [ ] Mobile-responsive design
- [ ] Offline mode capabilities
- [ ] Integration with language learning platforms



**Made with AI using Groq LLaMA-4 and Streamlit for emotion-aware language learning.**

© 2024 Your Name. All rights reserved.
