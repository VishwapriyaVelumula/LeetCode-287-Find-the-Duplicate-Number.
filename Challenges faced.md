
---

### 📄 `challenges_faced.md`  
```markdown
# Challenges Faced

1. **Space Constraint Clarification**  
   - The problem statement asks for “constant extra space,” but my initial frequency-array solution uses O(n) space.  
   - Realizing this, I explored Floyd’s cycle detection (tortoise & hare) to achieve true O(1) space.

2. **Choosing the Right Technique**  
   - Frequency array is conceptually simpler and runs in linear time, but doesn’t meet the strict space requirement.  
   - Implementing cycle detection correctly took careful pointer setup and edge-case thinking.

3. **Edge Cases**  
   - Arrays where the duplicate appears at the very start or end.  
   - Ensuring we never modify the input array when marking visits.

4. **Debugging Off-by-One Errors**  
   - The `nums` values range from **1** to **n**, but array indices are **0** to **n**.  
   - Accidentally mixing up these offsets resulted in runtime errors until corrected.

#Complexity
Time: O(n) — one pass through the array

Space: O(n) — auxiliary visit[] array (can be reduced to O(1) with cycle detection)
