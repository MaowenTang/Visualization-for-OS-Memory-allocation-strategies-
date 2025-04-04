# OS Memory Allocation Strategy Simulator

An interactive web-based simulator that demonstrates different memory allocation strategies in operating systems. This educational tool helps students understand how various memory allocation algorithms work and their impact on system performance.

## Overview

This simulator visualizes four common memory allocation strategies:
- First-Fit
- Next-Fit
- Best-Fit
- Worst-Fit

### Key Features

1. **Memory Configuration**
   - Total Memory: 10MB (10,240KB)
   - Block Size: 64KB per block
   - Total Blocks: 160 blocks
   - Pre-allocated OS Memory: 30-50% (randomly determined)

2. **Process Queue**
   - 200 processes with varied memory requirements
   - Size Categories:
     - Tiny (32-48KB): 25% - 50 processes
     - Small (49-96KB): 30% - 60 processes
     - Medium (97-160KB): 25% - 50 processes
     - Large (161-256KB): 15% - 30 processes
     - Very Large (257-384KB): 5% - 10 processes

3. **Dynamic Simulation**
   - Real-time process allocation
   - Random process completion (15% chance per cycle)
   - Continuous memory defragmentation
   - Side-by-side strategy comparison

4. **Performance Metrics**
   - Memory Utilization (%)
   - External Fragmentation (%)
   - Average Allocation Time (ms)
   - Success Rate
   - Total Cycles to Completion

## Technical Implementation

### Core Components

1. **Memory Manager Class**
   - Handles memory allocation logic
   - Tracks memory blocks and their status
   - Implements allocation strategies
   - Calculates performance metrics

2. **Process Class**
   - Stores process information
   - Tracks process status
   - Manages memory requirements

3. **Simulator Class**
   - Controls simulation flow
   - Manages process queue
   - Handles UI updates
   - Coordinates memory managers

### Memory Allocation Strategies

1. **First-Fit**
   - Allocates the first available space that fits
   - Quick but can lead to fragmentation
   - Implementation: Linear search from start

2. **Next-Fit**
   - Similar to First-Fit but continues from last position
   - Better distribution of allocations
   - Implementation: Circular search from last allocation

3. **Best-Fit**
   - Finds smallest suitable space
   - Minimizes wasted space
   - Implementation: Complete search for minimum viable space

4. **Worst-Fit**
   - Finds largest suitable space
   - Leaves large fragments
   - Implementation: Complete search for maximum space

### Visual Design

1. **Color Scheme**
   - Ghibli-inspired palette
   - Soft, nature-themed colors
   - High contrast for readability

2. **Layout**
   - 2×2 grid for strategies
   - Process queue visualization
   - Real-time statistics
   - Memory block visualization

3. **Interactive Elements**
   - Start/Reset controls
   - Step-by-step mode
   - Process tooltips
   - Memory block information

## Usage

1. **Setup**
   ```html
   <!-- Just open index.html in a modern web browser -->
   <!-- No server required - runs entirely in browser -->
   ```

2. **Controls**
   - "Start Comparison": Begin simulation
   - "Reset Simulation": Start fresh
   - "Step-by-step Mode": Manual advancement

3. **Visualization**
   - Colored blocks show memory status
   - Tooltips provide detailed information
   - Statistics update in real-time
   - Process queue shows allocation order

## Educational Value

1. **Concepts Demonstrated**
   - Memory allocation strategies
   - External fragmentation
   - Process scheduling
   - Resource utilization

2. **Observable Patterns**
   - Strategy efficiency differences
   - Fragmentation development
   - Allocation success rates
   - Performance trade-offs

3. **Learning Outcomes**
   - Understanding memory management
   - Comparing allocation strategies
   - Analyzing performance metrics
   - Visualizing system resources

## Technical Requirements

- Modern web browser with JavaScript enabled
- No external dependencies
- No server-side components needed
- Responsive design for various screen sizes

## Future Enhancements

1. **Potential Additions**
   - Custom memory configurations
   - More allocation strategies
   - Process priority system
   - Compaction algorithms

2. **Possible Improvements**
   - Advanced statistics
   - Performance optimizations
   - Additional visualization options
   - Export/import configurations

## License

MIT License - Feel free to use and modify for educational purposes.

## Credits

Designed and implemented as an educational tool for operating systems courses.
