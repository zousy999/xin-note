```java

    public static String format(Number number,String pattern,RoundingMode mode){
        if(number == null) return "0";
        DecimalFormat decimalFormat = new DecimalFormat(pattern);
        decimalFormat.setRoundingMode(mode);
        return decimalFormat.format(number);
    }

    public static String format(Number number,String pattern){
        return format(number,pattern,RoundingMode.HALF_UP);
    }

    /**
     * 四舍五入 保留两位小数 小数点后多余0 去除
     * @param number
     * @return
     */
    public static String format(Number number){
        return format(number,"##.##",RoundingMode.HALF_UP);
    }


    public static void main(String[] args) {
        System.out.println(format(2.124));//2.12
        System.out.println(format(2.125));//2.13
        System.out.println(format(2.996));//3
        System.out.println(format(2.004));//2
    }
```



