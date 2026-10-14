body {
  margin: 0;
  padding: 0;
  font-family: 'Poppins', sans-serif;
  background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 99%, #fecfef 100%);
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.container {
  background: rgba(255, 255, 255, 0.85);
  padding: 30px;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.15);
  max-width: 400px;
  width: 90%;
}

.title {
  color: #ff4757;
  font-size: 2rem;
  margin-bottom: 5px;
}

.name {
  color: #2f3542;
  margin-top: 0;
}

/* Cake & Candle Styles */
.cake-container {
  position: relative;
  width: 150px;
  height: 120px;
  margin: 40px auto 20px auto;
  cursor: pointer;
}

.cake {
  width: 150px;
  height: 90px;
  background: #ff6b81;
  border-radius: 10px 10px 0 0;
  position: absolute;
  bottom: 0;
}

.icing {
  width: 100%;
  height: 30px;
  background: #ffffff;
  border-radius: 10px 10px 15px 15px;
}

.candle {
  width: 12px;
  height: 40px;
  background: #ffa502;
  position: absolute;
  top: -10px;
  left: 50%;
  transform: translateX(-50%);
  border-radius: 3px;
}

.flame {
  width: 16px;
  height: 22px;
  background: #ff4757;
  border-radius: 50% 50% 20% 20%;
  position: absolute;
  top: -20px;
  left: -2px;
  box-shadow: 0 0 10px #ffa502;
  animation: flicker 0.5s infinite alternate;
}

@keyframes flicker {
  0% { transform: scale(1); }
  100% { transform: scale(1.15); }
}

.instruction {
  font-size: 0.9rem;
  color: #57606f;
}

/* Button & Surprise Box */
.btn {
  background-color: #ff4757;
  color: white;
  border: none;
  padding: 12px 24px;
  font-size: 1rem;
  font-weight: bold;
  border-radius: 25px;
  cursor: pointer;
  margin-top: 15px;
  transition: transform 0.2s, background-color 0.2s;
}

.btn:hover {
  background-color: #ff6b81;
  transform: scale(1.05);
}

.surprise-box {
  margin-top: 20px;
  padding: 15px;
  background: #ffffff;
  border-radius: 12px;
  border: 2px dashed #ff4757;
  animation: fadeIn 0.8s ease-in-out;
}

.hidden {
  display: none;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}
