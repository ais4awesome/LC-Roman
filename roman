def romanToInt(s: str) -> int:
        #s = "IV"   
        val = 0
        skip = False

        for r in s:
            if skip:
                skip = False
                continue
            else:
                if r == 'I':
                    if s.index(r) + 1 < len(s):
                        if s[s.index(r)+1] == 'V':
                            val = val + 4
                            skip = True
                        elif s[s.index(r)+1] == 'X':
                            val = val + 9
                            skip = True
                        else: 
                            val = val + 1
                    else: 
                        val = val + 1
                elif r == 'V':
                    val = val + 5
                elif r == 'X':
                    if s.index(r) + 1 < len(s):
                        if s[s.index(r)+1] == 'L':
                            val = val + 40
                            skip = True
                        elif s[s.index(r)+1] == 'C':
                            val = val + 90
                            skip = True
                        else: 
                            val = val + 10
                    else: 
                        val = val + 10
                elif r == 'L':
                    val = val + 50
                elif r == 'C':
                    if s.index(r) + 1 < len(s):
                        if s[s.index(r)+1] == 'D':
                            val = val + 400
                            skip = True
                        elif s[s.index(r)+1] == 'M':
                            val = val + 900
                            skip = True
                        else: 
                            val = val + 100
                    else: 
                        val = val + 100
                elif r == 'D':
                    val = val + 500
                elif r == 'M':
                    val = val + 1000
                
        return(val)
    
print(romanToInt("DCCLIII"))

# Optional approaches, break into functions, use switch statment, regex?