
import streamlit as st

st.title("Hoe Simulator 💀")
st.write(
    "How goes it fellows\n\n"
    "Welcome to Hoe Simulator!\n\n"
    "To see if you can get Hoes!"
)

# Initialize game state
if "question" not in st.session_state:
    st.session_state.question = 1

if "result" not in st.session_state:
    st.session_state.result = ""

def restart_game():
    st.session_state.question = 1
    st.session_state.result = ""

# Question 1
if st.session_state.question == 1:
    st.subheader("First Question!")
    st.write("You see the Hoes! What do you do?")

    if st.button("A: Tell them your name"):
        st.session_state.result = (
            "AHHHH scaring the hoes they don't care who you are\n"
            "Hoes Lost Try Again!"
        )
        st.session_state.question = 4

    if st.button("B: Show them your bandz with your elite money spread"):
        st.session_state.result = "Good Job you know hoes love the flex!"
        st.session_state.question = 2

    if st.button("C: Keep walking"):
        st.session_state.result = (
            "AHHH WRONG how u gon get the hoes???\n"
            "Hoes Lost Try Again!"
        )
        st.session_state.question = 4

# Question 2
elif st.session_state.question == 2:
    st.subheader("Next Question!")
    st.write("The hoes wanna do something. What should you take them to do?")

    if st.button("A: Bowling"):
        st.session_state.result = (
            "Wrong answer you know hoes cant bowl\n"
            "Hoes Lost Try Again!"
        )
        st.session_state.question = 4

    if st.button("B: Out to Eat"):
        st.session_state.result = "Good job you know hoes love to eat"
        st.session_state.question = 3

    if st.button("C: To your place"):
        st.session_state.result = (
            "WOOOOAH definelty scaring the hoes\n"
            "Hoes Lost Try Again!"
        )
        st.session_state.question = 4

# Question 3
elif st.session_state.question == 3:
    st.subheader("Last Question!")
    st.write("The Hoes wanna slide back to the crib! How do you bag the hoes?")

    if st.button("A: Show them your card collection"):
        st.session_state.result = (
            "HOES SECURED this young fellow knows how to get hoes"
        )
        st.session_state.question = 4

    if st.button("B: Whip it Out"):
        st.session_state.result = (
            "WHOOOOOAH definetley scaring the hoes\n"
            "Hoes Lost Try again!"
        )
        st.session_state.question = 4

    if st.button("C: Watch a movie with them"):
        st.session_state.result = (
            "AHHHHH bored the hoes they left\n"
            "Hoes Lost Try again!"
        )
        st.session_state.question = 4

# Display result
if st.session_state.result:
    st.write(st.session_state.result)

# Restart button
if st.session_state.question == 4:
    if st.button("Play Again 🔄"):
        restart_game()

        # Refresh the app
        st.rerun()
