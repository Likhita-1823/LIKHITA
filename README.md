# LIKHITA
resultUnit = 'C';
                    } else if (toUnit === 'K'){
                        convertedValue = (temperature - 273.15) * 9/5 +32;
                        resultUnit = 'K';
                    }else if (toUnit === 'R'){
                        convertedValue = temperature * 9/5;
                        resultUnit = 'R';
                    }else{
                        convertedValue = temperature;
                        resultUnit = 'K';
                    }
                    break;

                    case 'R':
                    if (toUnit === 'C'){
                        convertedValue = (temperature - 491.67) * 5/9;
                        resultUnit = 'C';
                    } else if (toUnit === 'K'){
                        convertedValue = temperature - 459.67;
                        resultUnit = 'K';
                    }else if (toUnit === 'R'){
                        convertedValue = temperature * 5/9;
                        resultUnit = 'R';
                    }else{
                        convertedValue = temperature;
                        resultUnit = 'R';
                    }
                    break;
            }

            document.getElementById('result').value = convertedValue.toFixed(2) + ' ' + resultUnit;
            
        }
    </script>
</body>

</html>
