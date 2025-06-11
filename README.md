import streamlit as st
st.set_page_config(page_title="🎵 SongPlay", layout="centered")
st.title("🎵 SongPlay")
st.write("Upload an MP3 file to play it:")
uploaded_file = st.file_uploader("Choose an MP3 file", type=["mp3"])
if uploaded_file is not None:
    st.audio(uploaded_file, format="audio/mp3")
    st.success(f"Now playing: {uploaded_file.name}")
else:
    st.info("Please upload an MP3 file.")
# soundplayer
a soundplayer
