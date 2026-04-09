# EngageLens: Advanced Classroom Intelligence Platform v2.0

![EngageLens Logo](https://img.shields.io/badge/EngageLens-Classroom%20AI-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-Production%20Ready-brightgreen)

**Advanced AI-driven classroom engagement analytics platform with high-granularity facial and behavioral tracking for educational research at SBBU SBA.**

---

## 🎯 Core Features

### 1. **Advanced Facial Tracking**
- ✅ **468-Point Face Mesh Detection** using MediaPipe for precision landmark tracking
- ✅ **3D Head Pose Estimation** (Yaw ±2°, Pitch ±2°, Roll ±2°)
- ✅ **Real-Time Expression Analysis** (Focused, Interested, Confused, Bored)
- ✅ **Eye Gaze & Pupil Tracking** for attention direction
- ✅ **Micro-Expression Detection** for subtle emotional shifts

### 2. **Behavioral Analytics**
- ✅ **Real-Time Engagement Scoring** (0-100% scale)
- ✅ **Gesture Recognition** (hand-to-face, fidgeting detection)
- ✅ **Posture Analysis** (slouch detection, alignment tracking)
- ✅ **Movement Velocity Analysis** for distraction patterns
- ✅ **Confidence Scoring** for all detections (0-1.0)

### 3. **Data Logging & Export**
- ✅ **Timestamped Behavioral Logs** with video correlation
- ✅ **JSON Export** for detailed analysis and research
- ✅ **CSV Export** for statistical processing and visualization
- ✅ **Session History** with aggregate metrics
- ✅ **Research-Grade Data Structure** for thesis analysis

### 4. **Real-Time Visualization**
- ✅ **Canvas Skeleton Overlay** showing facial mesh landmarks
- ✅ **Live Head Pose Indicators** with degree measurements
- ✅ **Expression Bar Charts** for engagement metrics
- ✅ **Engagement Timeline Graph** tracking changes over time
- ✅ **Alert System** for confusion, distraction, low engagement events

### 5. **Privacy & Security**
- ✅ **100% Local Processing** - no data sent to cloud
- ✅ **Browser-Based** - no server required
- ✅ **GDPR Compliant** - all data stored locally
- ✅ **Offline Capable** - works without internet

---

## 📊 Data Structure

### Behavioral Log Entry
```json
{
  "timestamp": "2026-04-09T10:02:04Z",
  "videoTime": 124,
  "headPose": {
    "yaw": 15.5,
    "pitch": -8.2,
    "roll": 3.1,
    "direction": "looking_left",
    "angleFromCenter": 15.5
  },
  "facialExpressions": {
    "focused": 45,
    "interested": 30,
    "confused": 15,
    "bored": 10,
    "dominant": "focused",
    "eyeOpenness": 72,
    "mouthOpenness": 8
  },
  "engagementScore": 78,
  "confidenceScore": 0.92,
  "alerts": ["minor_head_tilt_left"]
}
