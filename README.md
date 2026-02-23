# MSc Thesis Repository
### Efficient and Personalized Physical Activity Recommendations

Due to the signed Material Transfer Agreement with the UK Biobank, the raw data used in the predictive component of this repository cannot be publicly shared.

### Running the Demonstrator

1. Install Required Packages

Install the following Python packages using pip:
  - pandas
  - openai
  - tabulate


2. Required Files

Ensure the following files are located in the same folder:
  - cpa.csv – An adapted list of activities based on the Compendium of Physical Activities (included in the repository).
  - openai_key.txt – A text file containing your personal OpenAI API key.
  - met_values.csv – Sample user profiles with corresponding MET values (included in the repository).
  - llm_chatbot.py – The main Python script to run the demonstrator (included in the repository).


3. Running the Application

Execute llm_chatbot.py.
You will first be prompted to enter a User ID:
  - Enter 0 to simulate an active user.
  - Enter 1 to simulate a sedentary user.

The users listed in met_values.csv are pre-classified as either active or sedentary. The system automatically retrieves this classification along with the user’s corresponding MET value range.


4. Personalization Process

After selecting a User ID, the system will ask follow-up questions to tailor the recommendations. For example:
  - “I prefer outdoor activities. I want to improve my cardio, but I have knee problems.”

Based on the provided preferences, goals, and physiological considerations, the system generates personalized physical activity recommendations aligned with the user’s capabilities and objectives.



