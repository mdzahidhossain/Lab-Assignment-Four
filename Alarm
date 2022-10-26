public class Clock {
        private String hours;
        private String minutes;
        private int alarmHours;
        private int alarmMinutes;

        public Clock() {
        }

        public String getHours(){
            hours = java.time.LocalTime.now().toString().substring(0,2);
            return hours;
        }

        public String getMinutes(){
            minutes = java.time.LocalTime.now().toString().substring(3,5);
            return minutes;
        }

        public String getTime(){
            return getHours() + ":" + getMinutes();
        }

        public void setAlarm(int hour, int minutes){
            alarmHours = hour;
            alarmMinutes = minutes;
        }

        public String getAlarm(){
            if(Integer.parseInt(hours) >= alarmHours){
                if(Integer.parseInt(minutes) >= alarmMinutes){
                    alarmHours = 0;
                    alarmMinutes = 0;
                    return getTime() + " Alarm!!!";
                }
            } return getTime();
        }
    }
}
