# Exercise_shuhan
def VMTpcfunction(VMT, population, unit):
    if unit == "miles":
        VMTpercapita = VMT / population
    elif unit == "kilometers":
        VMTpercapita = (VMT / 1.60934) / population
    else:
        return "Invalid unit of measurement, use 'miles' or 'kilometers'"
    
    result = "Result:\nVMT=" + str(VMT) + "\nPopulation=" + str(population) + "\nUnit=" + unit + "\n\nVMT per capita = " + str(VMTpercapita)
    
    return result